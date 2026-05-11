import { useState } from "react";

export default function BigoRecruitmentPortal() {
  if (typeof window !== "undefined") {
    setTimeout(() => {
      const countdown = document.getElementById("countdown");

      if (countdown && !window.timerStarted) {
        window.timerStarted = true;

        let time = 300;

        const timer = setInterval(() => {
          const minutes = Math.floor(time / 60);
          const seconds = time % 60;

          countdown.innerHTML = `${minutes}:${seconds
            .toString()
            .padStart(2, "0")}`;

          time--;

          if (time < 0) {
            clearInterval(timer);
            countdown.innerHTML = "CLOSED";
          }
        }, 1000);
      }
    }, 100);
  }
  const [submitted, setSubmitted] = useState(false);
  const [applications, setApplications] = useState([]);
  const [showAdmin, setShowAdmin] = useState(false);

  const exportToExcel = () => {
    if (applications.length === 0) {
      alert("No applications available to export.");
      return;
    }

    const headers = [
      "Full Name",
      "Age",
      "Facebook",
      "Contact",
      "Address",
      "BIGO ID",
      "Government ID",
      "Email"
    ];

    const rows = applications.map((app) => [
      app.fullName,
      app.age,
      app.facebook,
      app.contact,
      app.address,
      app.bigoId,
      app.governmentId,
      app.email
    ]);

    const csvContent = [headers, ...rows]
      .map((e) => e.join(","))
      .join("\n");

    const blob = new Blob([csvContent], {
      type: "text/csv;charset=utf-8;"
    });

    const link = document.createElement("a");
    const url = URL.createObjectURL(blob);

    link.setAttribute("href", url);
    link.setAttribute("download", "TRD_BIGO_Applicants.csv");
    link.style.visibility = "hidden";

    document.body.appendChild(link);
    link.click();
    document.body.removeChild(link);
  };

  const handleSubmit = async (e) => {
    e.preventDefault();

    const formData = new FormData(e.target);

    const data = {
      fullName: formData.get("fullName"),
      age: formData.get("age"),
      facebook: formData.get("facebook"),
      contact: formData.get("contact"),
      address: formData.get("address"),
      bigoId: formData.get("bigoId"),
      governmentId: formData.get("governmentId"),
      email: formData.get("email"),
      reason: formData.get("reason")
    };

    const emailBody = `
NEW BIGO HOST APPLICATION

Full Name: ${data.fullName}
Age: ${data.age}
Facebook: ${data.facebook}
Contact Number: ${data.contact}
Address: ${data.address}
BIGO ID: ${data.bigoId}
Government ID: ${data.governmentId}
Email: ${data.email}

Reason for Applying:
${data.reason}
`;

    window.location.href = `mailto:crisnoel1217@gmail.com?subject=BIGO Host Application&body=${encodeURIComponent(emailBody)}`;

    setApplications((prev) => [...prev, data]);

    setSubmitted(true);
    e.target.reset();
  };
  return (
    <div className="min-h-screen bg-black text-white font-sans">
      {/* HERO SECTION */}
      <section className="relative overflow-hidden bg-gradient-to-br from-pink-600 via-purple-700 to-black">
        <div className="absolute inset-0 opacity-20 bg-[radial-gradient(circle_at_top_right,white,transparent_35%)]"></div>

        <div className="relative max-w-7xl mx-auto px-6 py-24 lg:py-32">
          <div className="grid lg:grid-cols-2 gap-12 items-center">
            <div>
              <div className="inline-flex items-center px-4 py-2 rounded-full bg-white/10 border border-white/20 mb-6 backdrop-blur-sm">
                <span className="text-sm font-semibold tracking-wide uppercase">
                  Join Our Agency Today
                </span>
              </div>

              <h1 className="text-5xl md:text-7xl font-black leading-tight mb-6">
                Become a
                <span className="block text-pink-300">BIGO Host</span>
              </h1>

              <p className="text-lg md:text-xl text-gray-200 max-w-xl mb-8 leading-relaxed">
                Start your streaming journey with a professional agency.
                Earn income, gain followers, receive training, and grow your
                online career with full support.
              </p>

              <div className="mt-8 mb-8 inline-block bg-white/10 border border-white/20 backdrop-blur-xl rounded-3xl px-8 py-6 shadow-2xl">
                <p className="text-sm uppercase tracking-[3px] text-pink-200 mb-2">
                  Recruitment Countdown
                </p>
                <h2
                  id="countdown"
                  className="text-5xl font-black text-yellow-300"
                >
                  05:00
                </h2>
              </div>

              <div className="grid grid-cols-2 gap-4 mb-10 max-w-2xl">
                <div className="bg-white/10 border border-white/20 backdrop-blur-xl rounded-3xl overflow-hidden shadow-2xl hover:scale-105 transition-all duration-300">
                  <img
                    src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?q=80&w=1200&auto=format&fit=crop"
                    alt="Singing Streamer"
                    className="w-full h-56 object-cover"
                  />

                  <div className="p-5">
                    <h3 className="text-2xl font-black mb-2">
                      🎤 Singing Streamer
                    </h3>
                    <p className="text-gray-200 text-sm leading-relaxed">
                      Showcase your voice live and earn gifts from fans worldwide.
                    </p>
                  </div>
                </div>

                <div className="bg-white/10 border border-white/20 backdrop-blur-xl rounded-3xl overflow-hidden shadow-2xl hover:scale-105 transition-all duration-300">
                  <img
                    src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?q=80&w=1200&auto=format&fit=crop"
                    alt="Dance Streamer"
                    className="w-full h-56 object-cover"
                  />

                  <div className="p-5">
                    <h3 className="text-2xl font-black mb-2">
                      💃 Dance Creator
                    </h3>
                    <p className="text-gray-200 text-sm leading-relaxed">
                      Go viral with live dance performances and interactive streams.
                    </p>
                  </div>
                </div>
              </div>

              <div className="flex flex-wrap gap-4">
                <a
                  href="#apply"
                  className="px-8 py-4 bg-white text-black rounded-2xl font-bold hover:scale-105 transition-all duration-300 shadow-2xl"
                >
                  Apply Now
                </a>

                <a
                  href="#benefits"
                  className="px-8 py-4 border border-white/30 rounded-2xl font-semibold hover:bg-white/10 transition-all duration-300"
                >
                  Learn More
                </a>
              </div>
            </div>

            <div className="relative">
              <div className="bg-white/10 border border-white/20 backdrop-blur-xl rounded-3xl p-8 shadow-2xl">
                <div className="space-y-6">
                  <div className="flex items-center justify-between">
                    <div>
                      <p className="text-sm text-gray-300">Monthly Potential</p>
                      <h3 className="text-4xl font-black">₱50K+</h3>
                    </div>
                    <div className="w-16 h-16 rounded-2xl bg-pink-500 flex items-center justify-center text-3xl">
                      🎤
                    </div>
                  </div>

                  <div className="grid grid-cols-2 gap-4">
                    <div className="bg-black/30 rounded-2xl p-5">
                      <h4 className="text-2xl font-bold">24/7</h4>
                      <p className="text-sm text-gray-300">Agency Support</p>
                    </div>

                    <div className="bg-black/30 rounded-2xl p-5">
                      <h4 className="text-2xl font-bold">1000+</h4>
                      <p className="text-sm text-gray-300">Active Hosts</p>
                    </div>
                  </div>

                  <div className="bg-gradient-to-r from-pink-500 to-purple-500 rounded-2xl p-5">
                    <p className="font-semibold text-lg">
                      No experience required.
                    </p>
                    <p className="text-sm text-pink-100 mt-1">
                      We provide complete guidance and mentoring.
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* BENEFITS */}
      <section id="benefits" className="max-w-7xl mx-auto px-6 py-24">
        <div className="text-center mb-16">
          <h2 className="text-4xl md:text-5xl font-black mb-4">
            Why Join Our Agency?
          </h2>
          <p className="text-gray-400 max-w-2xl mx-auto text-lg">
            We help aspiring creators become successful BIGO streamers through
            coaching, promotions, and premium support.
          </p>
        </div>

        <div className="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
          {[
            {
              title: "High Income",
              icon: "💰",
              desc: "Earn through streaming, gifts, and agency bonuses."
            },
            {
              title: "Training & Mentorship",
              icon: "🚀",
              desc: "Get expert guidance to grow faster on BIGO."
            },
            {
              title: "Flexible Schedule",
              icon: "⏰",
              desc: "Stream anytime and work from anywhere."
            },
            {
              title: "Friendly Community",
              icon: "🌟",
              desc: "Connect with supportive hosts and managers."
            }
          ].map((item, index) => (
            <div
              key={index}
              className="bg-zinc-900 border border-zinc-800 rounded-3xl p-8 hover:border-pink-500 hover:-translate-y-2 transition-all duration-300"
            >
              <div className="text-5xl mb-5">{item.icon}</div>
              <h3 className="text-2xl font-bold mb-3">{item.title}</h3>
              <p className="text-gray-400 leading-relaxed">{item.desc}</p>
            </div>
          ))}
        </div>
      </section>

      {/* REQUIREMENTS */}
      <section className="bg-zinc-950 py-24 px-6">
        <div className="max-w-6xl mx-auto grid lg:grid-cols-2 gap-16 items-center">
          <div>
            <h2 className="text-4xl md:text-5xl font-black mb-6">
              Basic Requirements
            </h2>

            <div className="space-y-5">
              {[
                "18 years old and above",
                "Stable internet connection",
                "Good communication skills",
                "Friendly and confident personality",
                "Passion for live streaming",
                "Must have a valid BIGO ID",
                "Must provide a valid government-issued ID"
              ].map((item, index) => (
                <div
                  key={index}
                  className="flex items-center gap-4 bg-black/30 rounded-2xl p-5 border border-zinc-800"
                >
                  <div className="w-10 h-10 rounded-full bg-pink-500 flex items-center justify-center font-bold">
                    ✓
                  </div>
                  <p className="text-lg">{item}</p>
                </div>
              ))}
            </div>
          </div>

          <div className="bg-gradient-to-br from-pink-600 to-purple-700 rounded-3xl p-10 shadow-2xl">
            <h3 className="text-3xl font-black mb-4">
              Ready to Start?
            </h3>

            <p className="text-pink-100 text-lg leading-relaxed mb-4">
              Apply now and our recruitment team will contact you for the next
              steps.
            </p>

            <div className="bg-white/10 border border-white/20 rounded-2xl p-4 mb-8">
              <p className="text-sm uppercase tracking-widest text-pink-200 mb-1">
                FOR INQUIRIES PLEASE CONTACT BIGO ID
              </p>
              <h4 className="text-2xl font-black">TRD10_28</h4>
            </div>

            <a
              href="#apply"
              className="inline-block px-8 py-4 bg-white text-black rounded-2xl font-bold hover:scale-105 transition-all duration-300"
            >
              Join the Agency
            </a>
          </div>
        </div>
      </section>

      {/* APPLICATION FORM */}
      <section id="apply" className="max-w-4xl mx-auto px-6 py-24">
        <div className="text-center mb-14">
          <h2 className="text-5xl font-black mb-4">Application Form</h2>
          <p className="text-gray-400 text-lg">
            Fill out the form below to apply as a BIGO Host.
          </p>
        </div>

        <form
          onSubmit={handleSubmit}
          className="bg-zinc-900 border border-zinc-800 rounded-3xl p-8 md:p-12 space-y-6 shadow-2xl"
        >
          <div className="grid md:grid-cols-2 gap-6">
            <div>
              <label className="block mb-2 text-sm text-gray-400">
                Full Name
              </label>
              <input
                name="fullName"
                type="text"
                required
                placeholder="Enter your full name"
                className="w-full bg-black border border-zinc-700 rounded-2xl px-5 py-4 outline-none focus:border-pink-500"
              />
            </div>

            <div>
              <label className="block mb-2 text-sm text-gray-400">
                Age
              </label>
              <input
                name="age"
                type="number"
                required
                placeholder="Enter your age"
                className="w-full bg-black border border-zinc-700 rounded-2xl px-5 py-4 outline-none focus:border-pink-500"
              />
            </div>
          </div>

          <div className="grid md:grid-cols-2 gap-6">
            <div>
              <label className="block mb-2 text-sm text-gray-400">
                Facebook Profile
              </label>
              <input
                name="facebook"
                type="text"
                required
                placeholder="Facebook link or name"
                className="w-full bg-black border border-zinc-700 rounded-2xl px-5 py-4 outline-none focus:border-pink-500"
              />
            </div>

            <div>
              <label className="block mb-2 text-sm text-gray-400">
                Contact Number
              </label>
              <input
                name="contact"
                type="text"
                required
                placeholder="09XXXXXXXXX"
                className="w-full bg-black border border-zinc-700 rounded-2xl px-5 py-4 outline-none focus:border-pink-500"
              />
            </div>
          </div>

          <div>
            <label className="block mb-2 text-sm text-gray-400">
              Complete Address
            </label>
            <input
              name="address"
              type="text"
              required
              placeholder="House No. / Street / Barangay / City / Province"
              className="w-full bg-black border border-zinc-700 rounded-2xl px-5 py-4 outline-none focus:border-pink-500"
            />
          </div>


          <div className="grid md:grid-cols-2 gap-6">
            <div>
              <label className="block mb-2 text-sm text-gray-400">
                BIGO ID
              </label>
              <input
                name="bigoId"
                type="text"
                required
                placeholder="Enter your BIGO ID"
                className="w-full bg-black border border-zinc-700 rounded-2xl px-5 py-4 outline-none focus:border-pink-500"
              />
            </div>

            <div>
              <label className="block mb-2 text-sm text-gray-400">
                Government ID Type
              </label>
              <select
                name="governmentId"
                required
                className="w-full bg-black border border-zinc-700 rounded-2xl px-5 py-4 outline-none focus:border-pink-500"
              >
                <option>Select Government ID</option>
                <option>Passport</option>
                <option>National ID</option>
                <option>Driver's License</option>
                <option>SSS ID</option>
                <option>PhilHealth ID</option>
                <option>TIN ID</option>
                <option>UMID</option>
                <option>Postal ID</option>
                <option>Voter's ID</option>
              </select>
            </div>
          </div>

          <div>
            <label className="block mb-2 text-sm text-gray-400">
              Email Address
            </label>
            <input
              name="email"
              type="email"
              required
              placeholder="Enter your email"
              className="w-full bg-black border border-zinc-700 rounded-2xl px-5 py-4 outline-none focus:border-pink-500"
            />
          </div>

          <div>
            <label className="block mb-2 text-sm text-gray-400">
              Why do you want to become a BIGO Host?
            </label>
            <textarea
              name="reason"
              rows="5"
              placeholder="Tell us about yourself..."
              className="w-full bg-black border border-zinc-700 rounded-2xl px-5 py-4 outline-none focus:border-pink-500"
            ></textarea>
          </div>

          <button
            type="submit"
            className="w-full py-5 bg-gradient-to-r from-pink-500 to-purple-600 rounded-2xl text-lg font-bold hover:scale-[1.02] transition-all duration-300"
          >
            {submitted ? "Application Sent Successfully" : "Submit Application"}
          </button>
        </form>
      </section>

      {/* TESTIMONIALS */}
      <section className="bg-zinc-950 py-24 px-6">
        <div className="max-w-7xl mx-auto">
          <div className="text-center mb-16">
            <h2 className="text-5xl font-black mb-4">
              Success Stories
            </h2>
            <p className="text-gray-400 text-lg">
              Hear from our successful BIGO hosts.
            </p>
          </div>

          <div className="grid md:grid-cols-3 gap-6">
            {[
              {
                name: "Alyssa",
                role: "Top Host",
                text: "Joining this agency helped me grow my followers and income quickly."
              },
              {
                name: "Kevin",
                role: "Gaming Streamer",
                text: "The support team guided me step-by-step from beginner to professional streamer."
              },
              {
                name: "Nicole",
                role: "Lifestyle Host",
                text: "Flexible schedule, supportive managers, and amazing opportunities."
              }
            ].map((item, index) => (
              <div
                key={index}
                className="bg-black border border-zinc-800 rounded-3xl p-8"
              >
                <div className="text-4xl mb-5">⭐</div>
                <p className="text-gray-300 leading-relaxed mb-6">
                  “{item.text}”
                </p>
                <div>
                  <h4 className="font-bold text-xl">{item.name}</h4>
                  <p className="text-pink-400">{item.role}</p>
                </div>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* FOOTER */}
      {/* ADMIN DASHBOARD */}
      <section className="max-w-7xl mx-auto px-6 py-24">
        <div className="flex items-center justify-between mb-10">
          <div>
            <h2 className="text-5xl font-black mb-3">
              Admin Dashboard
            </h2>
            <p className="text-gray-400 text-lg">
              View applicant summaries and recruitment data.
            </p>
          </div>

          <div className="flex gap-4 flex-wrap">
          <button
            onClick={exportToExcel}
            className="px-6 py-4 rounded-2xl bg-green-500 hover:scale-105 transition-all duration-300 font-bold"
          >
            Export to Excel
          </button>

          <button
            onClick={() => setShowAdmin(!showAdmin)}
            className="px-6 py-4 rounded-2xl bg-gradient-to-r from-pink-500 to-purple-600 font-bold"
          >
            {showAdmin ? "Hide Dashboard" : "Open Dashboard"}
          </button>
        </div>

        {showAdmin && (
          <div className="space-y-8">
            <div className="grid md:grid-cols-4 gap-6">
              <div className="bg-zinc-900 border border-zinc-800 rounded-3xl p-8">
                <p className="text-gray-400 mb-2">Total Applications</p>
                <h3 className="text-5xl font-black text-pink-400">
                  {applications.length}
                </h3>
              </div>

              <div className="bg-zinc-900 border border-zinc-800 rounded-3xl p-8">
                <p className="text-gray-400 mb-2">Agency</p>
                <h3 className="text-3xl font-black">
                  TRD Agency
                </h3>
              </div>

              <div className="bg-zinc-900 border border-zinc-800 rounded-3xl p-8">
                <p className="text-gray-400 mb-2">Reference BIGO ID</p>
                <h3 className="text-3xl font-black text-pink-400">
                  TRD10_28
                </h3>
              </div>

              <div className="bg-zinc-900 border border-zinc-800 rounded-3xl p-8">
                <p className="text-gray-400 mb-2">Recruitment Status</p>
                <h3 className="text-3xl font-black text-green-400">
                  OPEN
                </h3>
              </div>
            </div>

            <div className="bg-zinc-900 border border-zinc-800 rounded-3xl overflow-hidden">
              <div className="overflow-x-auto">
                <table className="w-full text-left">
                  <thead className="bg-black/40 border-b border-zinc-800">
                    <tr>
                      <th className="p-5">Name</th>
                      <th className="p-5">Age</th>
                      <th className="p-5">BIGO ID</th>
                      <th className="p-5">Contact</th>
                      <th className="p-5">Government ID</th>
                    </tr>
                  </thead>

                  <tbody>
                    {applications.length === 0 ? (
                      <tr>
                        <td colSpan="5" className="p-10 text-center text-gray-500">
                          No applications submitted yet.
                        </td>
                      </tr>
                    ) : (
                      applications.map((app, index) => (
                        <tr
                          key={index}
                          className="border-b border-zinc-800 hover:bg-black/20"
                        >
                          <td className="p-5 font-semibold">{app.fullName}</td>
                          <td className="p-5">{app.age}</td>
                          <td className="p-5 text-pink-400">{app.bigoId}</td>
                          <td className="p-5">{app.contact}</td>
                          <td className="p-5">{app.governmentId}</td>
                        </tr>
                      ))
                    )}
                  </tbody>
                </table>
              </div>
            </div>
          </div>
        )}
      </section>

      <footer className="border-t border-zinc-800 py-10 px-6 text-center">
        <h3 className="text-3xl font-black mb-2">TRD BIGO Agency</h3>
        <p className="text-gray-500">
          Empowering streamers and creators worldwide.
        </p>

        <div className="flex justify-center gap-6 mt-6 text-gray-400">
          <a href="#" className="hover:text-pink-400 transition">
            Facebook
          </a>
          <a href="#" className="hover:text-pink-400 transition">
            Telegram
          </a>
          <a href="#" className="hover:text-pink-400 transition">
            TikTok
          </a>
        </div>
      </footer>
    </div>
  );
}
