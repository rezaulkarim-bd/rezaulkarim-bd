import {
  FaGithub,
  FaReact,
  FaNodeJs,
  FaGitAlt,
} from "react-icons/fa";
import { SiTypescript, SiNextdotjs, SiMongodb } from "react-icons/si";

const HeroBanner = () => {
  return (
    <section className="w-full bg-gradient-to-r from-slate-100 via-blue-50 to-slate-200">
      <div className="mx-auto max-w-7xl px-4">
        <div className="relative flex min-h-[280px] items-center overflow-hidden rounded-2xl">

          {/* Left Decoration */}
          <div className="hidden w-[24%] flex-col items-center justify-center md:flex">
            <div className="rounded-full bg-gradient-to-r from-purple-300 to-cyan-300 px-5 py-2 text-sm font-semibold text-white shadow">
              Let's Collaborate!
            </div>

            <div className="mt-5 grid grid-cols-3 gap-5 text-2xl text-slate-600">
              <FaGithub />
              <FaReact />
              <SiTypescript />
              <SiNextdotjs />
              <FaNodeJs />
              <FaGitAlt />
            </div>
          </div>

          {/* Main Content */}
          <div className="z-10 flex-1 py-10 text-center md:text-left">
            <h1 className="text-4xl font-extrabold tracking-wide text-slate-900 md:text-5xl">
              Touhidur Zaman
            </h1>

            <h2 className="mt-1 text-xl font-bold text-slate-700 md:text-2xl">
              Full Stack Developer
            </h2>

            {/* Technology Icons */}
            <div className="mt-4 flex justify-center gap-4 text-xl text-slate-700 md:justify-start">
              <SiTypescript />
              <FaReact />
              <SiNextdotjs />
              <FaGitAlt />
              <SiMongodb />
              <FaNodeJs />
            </div>

            <p className="mt-4 text-sm font-medium text-slate-600">
              Turning ideas into clean, scalable web apps
            </p>

            {/* Contact */}
            <div className="mt-3 flex flex-col gap-1 text-xs text-slate-600 sm:flex-row sm:gap-5">
              <span>📧 touhidurcodes@gmail.com</span>
              <span>🌐 touhidurcodes.vercel.app</span>
            </div>
          </div>

          {/* Profile Image */}
          <div className="hidden h-full w-[25%] items-end justify-center md:flex">
            <img
              src="/profile.png"
              alt="Touhidur Zaman"
              className="h-[255px] w-auto object-contain"
            />
          </div>

        </div>
      </div>
    </section>
  );
};

export default HeroBanner;
