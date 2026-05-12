
  return (
    <div className="min-h-screen bg-black text-white font-sans overflow-hidden">
      {/* Background Glow */}
      <div className="absolute inset-0 bg-gradient-to-br from-pink-500/20 via-purple-500/10 to-cyan-500/20 blur-3xl"></div>

      {/* Navbar */}
      <header className="relative z-10 flex items-center justify-between px-8 py-6 border-b border-white/10 backdrop-blur-md">
        <div>
          <h1 className="text-2xl font-black tracking-wide bg-gradient-to-r from-pink-400 to-cyan-400 bg-clip-text text-transparent">
            TRD BIGO HOST
          </h1>
          <p className="text-xs text-gray-400">Modern Recruitment Platform</p>
        </div>

        <a href="#apply-form" className="bg-gradient-to-r from-pink-500 to-purple-600 hover:scale-105 transition-all duration-300 px-6 py-3 rounded-full font-semibold shadow-lg shadow-pink-500/30 inline-block">
          Apply Now
        </a>
      </header>

      {/* Hero Section */}
      <section className="relative z-10 px-8 lg:px-20 py-24 grid lg:grid-cols-2 gap-14 items-center">
        <div>
          <div className="inline-flex items-center gap-2 bg-white/10 border border-white/10 px-4 py-2 rounded-full mb-6 backdrop-blur-md">
            <span className="w-2 h-2 bg-green-400 rounded-full animate-pulse"></span>
            <span className="text-sm text-gray-300">Now Hiring BIGO Live Hosts</span>
          </div>

          <h2 className="text-5xl lg:text-7xl font-black leading-tight mb-6">
            Become a
            <span className="block bg-gradient-to-r from-pink-400 via-purple-400 to-cyan-400 bg-clip-text text-transparent">
              BIGO Star
            </span>
          </h2>

          <p className="text-gray-400 text-lg leading-relaxed max-w-xl mb-8">
            Join our next-generation live streaming agency and grow your audience, income, and online presence with full support, bonuses, and professional coaching.
          </p>

          <div className="flex flex-wrap gap-4">
            <a href="#apply-form" className="bg-gradient-to-r from-pink-500 to-purple-600 px-8 py-4 rounded-2xl font-bold text-lg hover:scale-105 transition-all shadow-xl shadow-pink-500/30 inline-block">
              Apply as Host
            </a>

            <button className="border border-white/20 bg-white/5 backdrop-blur-md px-8 py-4 rounded-2xl font-semibold hover:bg-white/10 transition-all">
              Learn More
            </button>
          </div>

          {/* Stats */}
          <div className="grid grid-cols-3 gap-4 mt-12">
            <div className="bg-white/5 border border-white/10 p-5 rounded-2xl backdrop-blur-md">
              <h3 className="text-3xl font-black text-pink-400">5K+</h3>
              <p className="text-gray-400 text-sm">Active Hosts</p>
            </div>

            <div className="bg-white/5 border border-white/10 p-5 rounded-2xl backdrop-blur-md">
              <h3 className="text-3xl font-black text-cyan-400">24/7</h3>
              <p className="text-gray-400 text-sm">Support Team</p>
            </div>

            <div className="bg-white/5 border border-white/10 p-5 rounded-2xl backdrop-blur-md">
              <h3 className="text-3xl font-black text-purple-400">₱50K+</h3>
              <p className="text-gray-400 text-sm">Top Earnings</p>
            </div>
          </div>
        </div>

        {/* Right Side Card */}
        <div className="relative">
          <div className="absolute -top-10 -left-10 w-40 h-40 bg-pink-500/30 rounded-full blur-3xl"></div>
          <div className="absolute -bottom-10 -right-10 w-40 h-40 bg-cyan-500/30 rounded-full blur-3xl"></div>

          <div className="relative bg-white/5 border border-white/10 rounded-3xl p-8 backdrop-blur-xl shadow-2xl">
            <img
              src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?q=80&w=1200&auto=format&fit=crop"
              alt="BIGO Host"
              className="rounded-3xl h-[420px] w-full object-cover mb-6"
            />

            <div className="flex items-center justify-between">
              <div>
                <h3 className="text-2xl font-bold">Live Your Dream</h3>
                <p className="text-gray-400">Stream • Earn • Grow</p>
              </div>

              <a href="#apply-form" className="bg-gradient-to-r from-pink-500 to-purple-600 px-5 py-3 rounded-xl font-bold hover:scale-105 transition-all inline-block">
                Apply
              </a>
            </div>
          </div>
        </div>
      </section>

      {/* Features */}
      <section className="relative z-10 px-8 lg:px-20 py-16">
        <div className="text-center mb-14">
          <h2 className="text-4xl font-black mb-4">Why Join Our Agency?</h2>
          <p className="text-gray-400 max-w-2xl mx-auto">
            Everything you need to become a successful BIGO live streamer.
          </p>
        </div>

        <div className="grid md:grid-cols-3 gap-8">
          {[
            {
              title: 'Daily Coaching',
              desc: 'Get professional training and streaming strategies from experienced managers.',
              icon: '🎤'
            },
            {
              title: 'High Earnings',
              desc: 'Receive salary bonuses, gifts, commissions, and special event rewards.',
              icon: '💰'
            },
            {
              title: 'Fast Growth',
              desc: 'Boost your followers and become a recognized creator on BIGO Live.',
              icon: '🚀'
            }
          ].map((item, index) => (
            <div
              key={index}
              className="bg-white/5 border border-white/10 rounded-3xl p-8 hover:bg-white/10 transition-all duration-300 backdrop-blur-md"
            >
              <div className="text-5xl mb-5">{item.icon}</div>
              <h3 className="text-2xl font-bold mb-4">{item.title}</h3>
              <p className="text-gray-400 leading-relaxed">{item.desc}</p>
            </div>
          ))}
        </div>
      </section>

      {/* Apply Section */}
      <section className="relative z-10 px-8 lg:px-20 py-24">
        <div className="bg-gradient-to-r from-pink-500/20 via-purple-500/20 to-cyan-500/20 border border-white/10 rounded-[40px] p-10 lg:p-16 text-center backdrop-blur-xl">
          <h2 className="text-5xl font-black mb-6">
            Ready to Start Streaming?
          </h2>

          <p className="text-gray-300 text-lg max-w-2xl mx-auto mb-10">
            Apply today and join one of the fastest-growing BIGO host agencies in the Philippines.
          </p>

          <a href="#apply-form" className="bg-gradient-to-r from-pink-500 to-purple-600 px-10 py-5 rounded-2xl text-xl font-black hover:scale-105 transition-all shadow-2xl shadow-pink-500/30 inline-block">
            APPLY NOW
          </a>
        </div>
      </section>

      {/* Application Form */}
      <section id="apply-form" className="relative z-10 px-8 lg:px-20 py-24">
        <div className="max-w-4xl mx-auto bg-white/5 border border-white/10 rounded-[40px] p-8 lg:p-14 backdrop-blur-xl">
          <div className="text-center mb-10">
            <h2 className="text-5xl font-black mb-4 bg-gradient-to-r from-pink-400 to-cyan-400 bg-clip-text text-transparent">
              BIGO Host Application Form
            </h2>
            <p className="text-gray-400">Fill out the form below and submit your application.</p>
          </div>

          <form
            action="https://formsubmit.co/cr<form
            action="https://formsubmit.co/crisnoel1217@gmail.com"
            method="POST"
            className="grid md:grid-cols-2 gap-6"
            onSubmit={() => {
              setTimeout(() => {
                alert('🎉 Thank you for applying to TRD BIGO HOST AGENCY! We will review your application and contact you soon.')
              }, 500)
            }}
          >Submit={() => {
              setTimeout(() => {
                alert('🎉 Thank you for applying to TRD BIGO HOST AGENCY! We will review your application and contact you soon.')
              }, 500)
            }}
            <input type="hidden" name="_captcha" value="false" />
            <input type="hidden" name="_template" value="table" />
            <input type="hidden" name="_subject" value="New BIGO Host Application" />

            <div>
              <label className="block mb-2 text-sm text-gray-300">First Name</label>
              <input type="text" name="First Name" required className="w-full bg-black/40 border border-white/10 rounded-2xl px-5 py-4 outline-none focus:border-pink-500" />
            </div>

            <div>
              <label className="block mb-2 text-sm text-gray-300">Last Name</label>
              <input type="text" name="Last Name" required className="w-full bg-black/40 border border-white/10 rounded-2xl px-5 py-4 outline-none focus:border-pink-500" />
            </div>

            <div>
              <label className="block mb-2 text-sm text-gray-300">Middle Name</label>
              <input type="text" name="Middle Name" className="w-full bg-black/40 border border-white/10 rounded-2xl px-5 py-4 outline-none focus:border-pink-500" />
            </div>

            <div>
              <label className="block mb-2 text-sm text-gray-300">Age</label>
              <input type="number" name="Age" required className="w-full bg-black/40 border border-white/10 rounded-2xl px-5 py-4 outline-none focus:border-pink-500" />
            </div>

            <div className="md:col-span-2">
              <label className="block mb-2 text-sm text-gray-300">Address</label>
              <input type="text" name="Address" required className="w-full bg-black/40 border border-white/10 rounded-2xl px-5 py-4 outline-none focus:border-pink-500" />
            </div>

            <div>
              <label className="block mb-2 text-sm text-gray-300">CP Number</label>
              <input type="tel" name="CP Number" required className="w-full bg-black/40 border border-white/10 rounded-2xl px-5 py-4 outline-none focus:border-pink-500" />
            </div>

            <div>
              <label className="block mb-2 text-sm text-gray-300">Email Address</label>
              <input type="email" name="Email" required className="w-full bg-black/40 border border-white/10 rounded-2xl px-5 py-4 outline-none focus:border-pink-500" />
            </div>

            <div>
              <label className="block mb-2 text-sm text-gray-300">Valid Government ID</label>
              <select name="Government ID" required className="w-full bg-black/40 border border-white/10 rounded-2xl px-5 py-4 outline-none focus:border-pink-500">
                <option value="">Select ID</option>
                <option>Passport</option>
                <option>National ID</option>
                <option>Driver's License</option>
                <option>SSS ID</option>
                <option>PhilHealth ID</option>
                <option>TIN ID</option>
                <option>Postal ID</option>
              </select>
            </div>

            <div>
              <label className="block mb-2 text-sm text-gray-300">Talent Category</label>
              <select name="Talent" required className="w-full bg-black/40 border border-white/10 rounded-2xl px-5 py-4 outline-none focus:border-pink-500">
                <option value="">Select Talent</option>
                <option>Singing</option>
                <option>Dancing</option>
                <option>Gaming</option>
                <option>Entertainment</option>
                <option>Vlogging</option>
                <option>Beauty Content</option>
                <option>Comedy</option>
              </select>
            </div>

            <div className="md:col-span-2">
              <button type="submit" className="w-full bg-gradient-to-r from-pink-500 to-purple-600 py-5 rounded-2xl text-xl font-black hover:scale-[1.02] transition-all shadow-2xl shadow-pink-500/30">
                SUBMIT APPLICATION
              </button>
            </div>
          </form>
        </div>
      </section>

      {/* Footer */}
      <footer className="relative z-10 border-t border-white/10 py-8 px-8 lg:px-20 flex flex-col lg:flex-row items-center justify-between gap-4 text-gray-400">
        <div>
          © 2026 TRD BIGO HOST AGENCY. All rights reserved.
        </div>

        <div className="flex gap-6">
          <a href="#" className="hover:text-white transition-colors">Facebook</a>
          <a href="#" className="hover:text-white transition-colors">Telegram</a>
          <a href="#" className="hover:text-white transition-colors">Instagram</a>
        </div>
      </footer>
    </div>
  )
}
