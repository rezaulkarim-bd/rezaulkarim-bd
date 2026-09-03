import {
  Github,
  Linkedin,
  Mail,
  Code2,
  Atom,
  Triangle,
  Braces,
} from "lucide-react"

const ProfileBanner = () => {
  return (
    <section className="relative min-h-[300px] w-full overflow-hidden bg-gradient-to-r from-slate-100 via-blue-50 to-slate-200">
      
      {/* Background decoration */}
      <div className="absolute left-0 top-0 h-full w-full opacity-30">
        <div className="absolute left-[10%] top-[15%] h-2 w-2 rounded-full bg-slate-500" />
        <div className="absolute left-[25%] top-[30%] h-2 w-2 rounded-full bg-slate-500" />
        <div className="absolute left-[40%] top-[10%] h-2 w-2 rounded-full bg-slate-500" />
        <div className="absolute left-[55%] top-[35%] h-2 w-2 rounded-full bg-slate-500" />
      </div>

      <div className="relative mx-auto flex min-h-[300px] max-w-7xl items-center justify-between px-6 py-10 md:px-12">
        
        {/* Left Content */}
        <div className="z-10 max-w-3xl">
          
          {/* Badge */}
          <div className="mb-6 inline-block rounded-full bg-gradient-to-r from-purple-500 to-blue-400 px-6 py-3 font-bold text-white shadow-lg">
            Let's Collaborate!
          </div>

          {/* Name */}
          <h1 className="text-4xl font-extrabold tracking-wide text-slate-800 md:text-6xl">
            Your Name
          </h1>

          {/* Designation */}
          <h2 className="mt-2 text-xl font-bold text-slate-700 md:text-2xl">
            Full Stack Developer
          </h2>

          {/* Tech Icons */}
          <div className="mt-8 flex flex-wrap items-center gap-5 text-slate-600">
            <Code2 size={32} />
            <Atom size={32} />
            <Triangle size={30} />
            <Braces size={32} />
            <Github size={30} />
          </div>

          <p className="mt-5 text-base font-medium text-slate-600 md:text-lg">
            Turning ideas into clean, scalable web apps
          </p>

          {/* Contact */}
          <div className="mt-5 flex flex-wrap items-center gap-5 text-sm text-slate-600">
            <a
              href="mailto:your@email.com"
              className="flex items-center gap-2 hover:text-blue-600"
            >
              <Mail size={16} />
              your@email.com
            </a>

            <a
              href="https://github.com/yourusername"
              className="flex items-center gap-2 hover:text-blue-600"
            >
              <Github size={16} />
              github.com/yourusername
            </a>

            <a
              href="https://linkedin.com"
              className="flex items-center gap-2 hover:text-blue-600"
            >
              <Linkedin size={16} />
              LinkedIn
            </a>
          </div>
        </div>

        {/* Right Image */}
        <div className="relative z-10 hidden self-end md:block">
          <img
            src="YOUR_IMAGE_URL"
            alt="Profile"
            className="h-[270px] w-[220px] object-cover object-top"
          />
        </div>
      </div>
    </section>
  )
}

export default ProfileBanner
