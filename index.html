import { useState, useEffect } from "react";

const GlobalStyle = () => (
  <style>{`
    @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=DM+Sans:wght@300;400;500&display=swap');

    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    :root {
      --gold:      #C9974A;
      --gold-light:#F0C060;
      --black:     #0A0804;
      --dark:      #130F08;
      --card:      #1A1508;
      --surface:   #201A0C;
      --border:    rgba(201,151,74,.25);
      --text:      #F5EDD8;
      --muted:     rgba(245,237,216,.5);
    }

    body { background: var(--black); font-family: 'DM Sans', sans-serif; color: var(--text); }
    .serif { font-family: 'Playfair Display', serif; }

    .shell {
      width: 390px; min-height: 844px; max-height: 844px;
      margin: 32px auto; border-radius: 44px;
      box-shadow: 0 0 0 10px #1a1508, 0 0 0 11px #C9974A44, 0 40px 100px rgba(0,0,0,.8);
      overflow: hidden; position: relative;
      display: flex; flex-direction: column; background: var(--black);
    }

    .screen {
      flex: 1; overflow-y: auto; overflow-x: hidden;
      scroll-behavior: smooth; padding-bottom: 80px;
    }
    .screen::-webkit-scrollbar { display: none; }

    .nav {
      position: absolute; bottom: 0; left: 0; right: 0; height: 72px;
      background: rgba(10,8,4,.97); backdrop-filter: blur(12px);
      border-top: 1px solid var(--border);
      display: flex; align-items: center; justify-content: space-around; z-index: 100;
    }
    .nav-btn {
      display: flex; flex-direction: column; align-items: center; gap: 4px;
      background: none; border: none; cursor: pointer;
      font-family: 'DM Sans', sans-serif; font-size: 10px; font-weight: 500;
      color: var(--muted); padding: 8px 12px; border-radius: 12px; transition: all .2s;
    }
    .nav-btn.active { color: var(--gold); }
    .nav-btn svg { width: 22px; height: 22px; stroke-width: 1.8; }

    .btn-gold {
      background: linear-gradient(135deg, #C9974A, #F0C060); color: #0A0804;
      border: none; border-radius: 30px; padding: 14px 28px;
      font-family: 'DM Sans', sans-serif; font-size: 14px; font-weight: 700;
      cursor: pointer; transition: transform .15s, box-shadow .15s;
      box-shadow: 0 4px 24px rgba(201,151,74,.4); letter-spacing: .3px;
    }
    .btn-gold:hover { transform: translateY(-2px); box-shadow: 0 8px 32px rgba(201,151,74,.55); }

    .btn-outline {
      background: transparent; color: var(--gold);
      border: 1.5px solid var(--gold); border-radius: 30px;
      padding: 12px 24px; font-family: 'DM Sans', sans-serif;
      font-size: 13px; font-weight: 500; cursor: pointer; transition: all .2s;
    }
    .btn-outline:hover { background: var(--gold); color: var(--black); }

    input, textarea {
      width: 100%; padding: 14px 16px; border: 1.5px solid var(--border);
      border-radius: 14px; background: var(--surface);
      font-family: 'DM Sans', sans-serif; font-size: 14px; color: var(--text);
      outline: none; transition: border .2s; resize: none;
    }
    input:focus, textarea:focus { border-color: var(--gold); }
    input::placeholder, textarea::placeholder { color: var(--muted); }
    label { font-size: 12px; font-weight: 500; color: var(--muted); margin-bottom: 6px; display: block; }

    .tag {
      display: inline-block; background: rgba(201,151,74,.15); color: var(--gold);
      font-size: 11px; font-weight: 600; padding: 4px 10px; border-radius: 20px;
      border: 1px solid rgba(201,151,74,.3);
    }

    .gold-line {
      height: 1px; background: linear-gradient(90deg, transparent, var(--gold), transparent); margin: 0 20px;
    }

    /* Popup */
    .popup-overlay {
      position: absolute; inset: 0; background: var(--black);
      display: flex; flex-direction: column;
      align-items: center; justify-content: center; z-index: 999;
    }
    @keyframes popUp {
      0%   { transform: scale(.5) translateY(40px); opacity: 0 }
      65%  { transform: scale(1.07) translateY(-6px); opacity: 1 }
      100% { transform: scale(1) translateY(0); opacity: 1 }
    }
    @keyframes shimmer {
      0%   { background-position: -200% center }
      100% { background-position: 200% center }
    }
    @keyframes barGrow { from { width: 0 } to { width: 140px } }
    .logo-pop { animation: popUp .75s cubic-bezier(.34,1.56,.64,1) forwards; }

    /* Steps */
    .step-row { display: flex; gap: 0; padding: 0 20px; }
    .step-item { flex: 1; text-align: center; position: relative; }
    .step-item:not(:last-child)::after {
      content: ''; position: absolute; top: 20px; right: 0;
      width: 50%; height: 1px; background: linear-gradient(90deg, var(--gold), transparent);
    }
    .step-num {
      width: 40px; height: 40px; border-radius: 50%;
      background: linear-gradient(135deg, #C9974A, #F0C060); color: var(--black);
      display: flex; align-items: center; justify-content: center;
      font-weight: 700; font-size: 16px; margin: 0 auto 10px;
      box-shadow: 0 4px 16px rgba(201,151,74,.4);
    }

    /* Cards */
    .event-card {
      background: var(--card); border-radius: 20px;
      padding: 20px; margin: 0 20px 16px; border: 1px solid var(--border);
    }
    .ann-card {
      background: var(--card); border-radius: 20px;
      margin: 0 20px 16px; overflow: hidden; border: 1px solid var(--border);
    }

    /* Settings toggle */
    .toggle {
      width: 44px; height: 24px; border-radius: 12px;
      border: none; cursor: pointer; position: relative; transition: background .2s;
    }
    .toggle::after {
      content: ''; position: absolute; width: 18px; height: 18px; border-radius: 50%;
      background: #fff; top: 3px; transition: left .2s; box-shadow: 0 1px 4px rgba(0,0,0,.4);
    }
    .toggle.on { background: linear-gradient(135deg,#C9974A,#F0C060); }
    .toggle.on::after { left: 23px; }
    .toggle.off { background: #333; }
    .toggle.off::after { left: 3px; }

    .settings-row {
      display: flex; align-items: center; justify-content: space-between;
      padding: 16px 20px; border-bottom: 1px solid var(--border); background: var(--card);
    }

    .photo-strip {
      display: flex; gap: 12px; padding: 0 20px;
      overflow-x: auto; scroll-snap-type: x mandatory;
    }
    .photo-strip::-webkit-scrollbar { display: none; }
    .photo-item {
      flex-shrink: 0; width: 160px; height: 200px;
      border-radius: 18px; scroll-snap-align: start;
      border: 1px solid var(--border);
      display: flex; flex-direction: column; align-items: center; justify-content: center; gap: 8px;
    }
  `}</style>
);

const Icon = ({ name }) => {
  const icons = {
    home:     <><path d="M3 9.5L12 3l9 6.5V20a1 1 0 01-1 1H4a1 1 0 01-1-1V9.5z"/><path d="M9 21V12h6v9"/></>,
    announce: <><rect x="3" y="5" width="18" height="14" rx="2"/><path d="M3 9h18M9 5v4M15 5v4"/></>,
    book:     <><rect x="4" y="4" width="16" height="16" rx="2"/><path d="M8 2v4M16 2v4M4 10h16"/></>,
    profile:  <><circle cx="12" cy="8" r="4"/><path d="M4 20c0-4 3.6-7 8-7s8 3 8 7"/></>,
  };
  return <svg viewBox="0 0 24 24" fill="none" stroke="currentColor">{icons[name]}</svg>;
};

const GoldText = ({ children, size = 16, serif = false, style = {} }) => (
  <span className={serif ? "serif" : ""} style={{
    fontSize: size, fontWeight: 700,
    background: "linear-gradient(135deg, #C9974A 0%, #F0C060 50%, #C9974A 100%)",
    backgroundSize: "200% auto",
    WebkitBackgroundClip: "text", WebkitTextFillColor: "transparent",
    animation: "shimmer 3s linear infinite", ...style
  }}>{children}</span>
);

const NaariLogo = ({ size = 56 }) => (
  <div style={{ textAlign: "center" }}>
    <div style={{ display: "flex", alignItems: "baseline", justifyContent: "center", gap: 1 }}>
      <GoldText serif size={size} style={{ letterSpacing: "-1px", lineHeight: 1 }}>नारी</GoldText>
      <span className="serif" style={{
        fontSize: size, fontWeight: 700, letterSpacing: "-1px", lineHeight: 1, color: "#fff"
      }}>First</span>
    </div>
    <div style={{ fontSize: size * 0.19, letterSpacing: "3px", textTransform: "uppercase",
      color: "rgba(201,151,74,.55)", marginTop: 6 }}>
      Women · Community · Power
    </div>
  </div>
);

const Corner = ({ top, right, bottom, left }) => (
  <div style={{
    position: "absolute", width: 22, height: 22,
    top, right, bottom, left,
    borderTop: top !== undefined ? "1px solid #C9974A55" : "none",
    borderBottom: bottom !== undefined ? "1px solid #C9974A55" : "none",
    borderLeft: left !== undefined ? "1px solid #C9974A55" : "none",
    borderRight: right !== undefined ? "1px solid #C9974A55" : "none",
  }} />
);

// ── POPUP ─────────────────────────────────────────────────────────────────────
const LogoPopup = ({ onDone }) => {
  useEffect(() => { const t = setTimeout(onDone, 2600); return () => clearTimeout(t); }, []);
  return (
    <div className="popup-overlay">
      <Corner top={28} left={28} /> <Corner top={28} right={28} />
      <Corner bottom={28} left={28} /> <Corner bottom={28} right={28} />
      <div className="logo-pop"><NaariLogo size={60} /></div>
      <div style={{ marginTop: 32, height: 1, animation: "barGrow .9s 1s ease forwards", width: 0,
        background: "linear-gradient(90deg,transparent,#C9974A,#F0C060,#C9974A,transparent)" }}/>
      <div style={{ marginTop: 20, color: "rgba(201,151,74,.45)", fontSize: 11,
        letterSpacing: "4px", textTransform: "uppercase" }}>Est. 2025</div>
    </div>
  );
};

// ── AUTH ──────────────────────────────────────────────────────────────────────
const AuthScreen = ({ onAuth }) => {
  const [mode, setMode] = useState("login");
  const [form, setForm] = useState({ name: "", email: "", password: "" });

  return (
    <div style={{ minHeight: 844, background: "radial-gradient(ellipse at 30% 20%,#1a1200,#0A0804 65%)",
      display: "flex", flexDirection: "column", alignItems: "center",
      justifyContent: "flex-end", padding: "40px 28px", position: "relative", overflow: "hidden" }}>

      <div style={{ position: "absolute", top: 0, left: "50%", transform: "translateX(-50%)",
        width: 320, height: 320, borderRadius: "50%",
        background: "radial-gradient(circle,rgba(201,151,74,.1),transparent 70%)", pointerEvents: "none" }}/>

      <div style={{ position: "absolute", top: 90, left: "50%", transform: "translateX(-50%)", width: "100%" }}>
        <NaariLogo size={50} />
      </div>

      <div style={{ width: "100%", background: "rgba(201,151,74,.07)", backdropFilter: "blur(20px)",
        borderRadius: 28, border: "1px solid rgba(201,151,74,.2)", padding: "28px 24px" }}>
        <div style={{ display: "flex", background: "rgba(0,0,0,.4)",
          borderRadius: 20, padding: 4, marginBottom: 24 }}>
          {["login","signup"].map(m => (
            <button key={m} onClick={() => setMode(m)} style={{
              flex: 1, padding: "10px 0", border: "none", borderRadius: 16, cursor: "pointer",
              fontFamily: "'DM Sans',sans-serif", fontSize: 14, fontWeight: 600, transition: "all .2s",
              background: mode === m ? "linear-gradient(135deg,#C9974A,#F0C060)" : "transparent",
              color: mode === m ? "#0A0804" : "rgba(201,151,74,.6)"
            }}>{m === "login" ? "Sign In" : "Sign Up"}</button>
          ))}
        </div>

        <div style={{ display: "flex", flexDirection: "column", gap: 14 }}>
          {mode === "signup" && (
            <div><label>Full Name</label>
              <input placeholder="Your name" onChange={e => setForm(p=>({...p,name:e.target.value}))}/></div>
          )}
          <div><label>Email</label>
            <input type="email" placeholder="you@email.com" onChange={e => setForm(p=>({...p,email:e.target.value}))}/></div>
          <div><label>Password</label>
            <input type="password" placeholder="••••••••" onChange={e => setForm(p=>({...p,password:e.target.value}))}/></div>
          <button className="btn-gold" onClick={onAuth} style={{ marginTop: 8, width: "100%" }}>
            {mode === "login" ? "Sign In →" : "Create Account →"}
          </button>
        </div>
        <p style={{ textAlign: "center", color: "rgba(201,151,74,.35)", fontSize: 12, marginTop: 20 }}>
          ✦ By joining you agree to our community values ✦
        </p>
      </div>
    </div>
  );
};

const events = [
  { id:1, name:"Bloom Summit 2025", date:"June 14, 2025", place:"Mumbai", emoji:"🌸",
    text:"A full-day summit on women in leadership, entrepreneurship & wellness.",
    bg:"linear-gradient(135deg,#1a1200,#3d2e00)" },
  { id:2, name:"Naari Nights", date:"July 5, 2025", place:"Delhi", emoji:"✨",
    text:"An intimate evening of storytelling, connection & celebration.",
    bg:"linear-gradient(135deg,#0a0804,#201500)" },
  { id:3, name:"The Circle — Mentorship", date:"July 22, 2025", place:"Online", emoji:"💡",
    text:"Match with senior mentors for 1:1 sessions across industries.",
    bg:"linear-gradient(135deg,#2e2000,#5a3e00)" },
];
const vibePhotos = [
  { bg:"linear-gradient(135deg,#1a1200,#3d2e00)", emoji:"🌸", label:"Networking" },
  { bg:"linear-gradient(135deg,#0a0804,#2a1f00)", emoji:"✨", label:"Events" },
  { bg:"linear-gradient(135deg,#2e2000,#5a3e00)", emoji:"🌿", label:"Wellness" },
  { bg:"linear-gradient(135deg,#1a1508,#3d2e00)", emoji:"💼", label:"Leadership" },
];

// ── HOME ──────────────────────────────────────────────────────────────────────
const HomePage = ({ onRSVP }) => (
  <div>
    <div style={{ background:"radial-gradient(ellipse at 50% 0%,#2a1f00,#0a0804 80%)",
      padding:"60px 28px 52px", textAlign:"center", position:"relative", overflow:"hidden",
      borderBottom:"1px solid var(--border)" }}>
      <Corner top={20} left={20}/><Corner top={20} right={20}/>
      <span className="tag" style={{ marginBottom:20, display:"inline-block" }}>✦ Exclusive Community</span>
      <h1 className="serif" style={{ fontSize:36, lineHeight:1.15, marginBottom:14 }}>
        <span style={{ background:"linear-gradient(160deg,#fff 0%,#F0C060 60%,#C9974A 100%)",
          WebkitBackgroundClip:"text", WebkitTextFillColor:"transparent" }}>
          नारीFirst is<br/><em>where women<br/>rise together.</em>
        </span>
      </h1>
      <p style={{ color:"var(--muted)", fontSize:14, lineHeight:1.6,
        maxWidth:280, margin:"0 auto 28px" }}>
        A curated space for ambitious women to connect, grow & celebrate each other.
      </p>
      <button className="btn-gold" onClick={onRSVP}>Join / Request Invite</button>
    </div>

    <div style={{ padding:"28px 20px 0" }}>
      <p style={{ fontSize:11, fontWeight:600, letterSpacing:"2px", textTransform:"uppercase",
        color:"var(--gold)", marginBottom:12, opacity:.7 }}>Next Event</p>
      <div className="event-card" style={{ margin:0, display:"flex",
        justifyContent:"space-between", alignItems:"center" }}>
        <div>
          <div className="serif" style={{ fontSize:18, fontWeight:700, color:"var(--text)", marginBottom:6 }}>
            Bloom Summit 2025</div>
          <div style={{ fontSize:13, color:"var(--muted)" }}>📅 June 14 · Mumbai</div>
        </div>
        <button className="btn-gold" style={{ padding:"10px 18px", fontSize:13 }} onClick={onRSVP}>RSVP</button>
      </div>
    </div>

    <div style={{ padding:"32px 0 0" }}>
      <p style={{ fontSize:11, fontWeight:600, letterSpacing:"2px", textTransform:"uppercase",
        color:"var(--gold)", marginBottom:14, paddingLeft:20, opacity:.7 }}>The Vibe</p>
      <div className="photo-strip">
        {vibePhotos.map((p,i) => (
          <div key={i} className="photo-item" style={{ background:p.bg }}>
            <div style={{ fontSize:44 }}>{p.emoji}</div>
            <div style={{ color:"var(--gold)", fontSize:11, fontWeight:600,
              letterSpacing:"2px", textTransform:"uppercase" }}>{p.label}</div>
          </div>
        ))}
      </div>
    </div>

    <div style={{ padding:"36px 0 0" }}>
      <p style={{ fontSize:11, fontWeight:600, letterSpacing:"2px", textTransform:"uppercase",
        color:"var(--gold)", marginBottom:20, textAlign:"center", opacity:.7 }}>How It Works</p>
      <div className="step-row">
        {[["Join","Apply to our community"],["Get Invite","We review & welcome you"],["Attend","Show up & shine ✦"]].map(([t,s],i) => (
          <div key={i} className="step-item">
            <div className="step-num">{i+1}</div>
            <div style={{ fontSize:12, fontWeight:600, color:"var(--text)", marginBottom:4 }}>{t}</div>
            <div style={{ fontSize:10, color:"var(--muted)", lineHeight:1.4 }}>{s}</div>
          </div>
        ))}
      </div>
    </div>

    <div style={{ margin:"36px 20px 0", padding:"28px 24px",
      background:"linear-gradient(135deg,#1a1200,#2e2000)",
      borderRadius:24, textAlign:"center", border:"1px solid rgba(201,151,74,.3)" }}>
      <GoldText size={24} style={{ display:"block", marginBottom:14 }}>✦</GoldText>
      <p className="serif" style={{ fontSize:16, lineHeight:1.7, fontStyle:"italic",
        background:"linear-gradient(135deg,#F0C060,#C9974A)",
        WebkitBackgroundClip:"text", WebkitTextFillColor:"transparent" }}>
        "We exist to lift women up — through community, opportunity, and radical sisterhood."
      </p>
      <div style={{ marginTop:14, color:"rgba(201,151,74,.5)", fontSize:12,
        letterSpacing:"2px", textTransform:"uppercase" }}>The NaariFirst Mission</div>
    </div>

    <div style={{ margin:"28px 20px 0", padding:"28px 24px", background:"var(--card)",
      borderRadius:20, textAlign:"center", border:"1px solid var(--border)" }}>
      <NaariLogo size={26}/>
      <div className="gold-line" style={{ margin:"20px 0" }}/>
      <div style={{ display:"flex", justifyContent:"center", gap:20 }}>
        <a href="#" style={{ color:"var(--muted)", fontSize:12, textDecoration:"none" }}>📧 hello@naarifirst.com</a>
        <a href="#" style={{ color:"var(--muted)", fontSize:12, textDecoration:"none" }}>📸 @entreprenaari.com</a>
      </div>
    </div>
  </div>
);

// ── ANNOUNCEMENTS ─────────────────────────────────────────────────────────────
const AnnouncementPage = ({ onRSVP }) => (
  <div>
    <div style={{ padding:"32px 20px 20px" }}>
      <p style={{ fontSize:11, fontWeight:600, letterSpacing:"2px", textTransform:"uppercase",
        color:"var(--gold)", marginBottom:4, opacity:.7 }}>Upcoming</p>
      <h2 className="serif" style={{ fontSize:28, fontWeight:700,
        background:"linear-gradient(135deg,#fff,#F0C060)",
        WebkitBackgroundClip:"text", WebkitTextFillColor:"transparent" }}>Events</h2>
    </div>
    {events.map(e => (
      <div key={e.id} className="ann-card">
        <div style={{ height:140, background:e.bg, display:"flex", alignItems:"center",
          justifyContent:"center", fontSize:48, borderBottom:"1px solid var(--border)" }}>{e.emoji}</div>
        <div style={{ padding:"16px 18px" }}>
          <div style={{ display:"flex", justifyContent:"space-between", alignItems:"flex-start", marginBottom:8 }}>
            <div>
              <div className="serif" style={{ fontSize:17, fontWeight:700, color:"var(--text)" }}>{e.name}</div>
              <div style={{ fontSize:12, color:"var(--muted)", marginTop:4 }}>📅 {e.date} · 📍 {e.place}</div>
            </div>
            <span className="tag">New</span>
          </div>
          <p style={{ fontSize:13, color:"var(--muted)", lineHeight:1.55, marginBottom:14 }}>{e.text}</p>
          <button className="btn-gold" style={{ padding:"10px 22px", fontSize:13 }}
            onClick={() => onRSVP(e)}>RSVP →</button>
        </div>
      </div>
    ))}
    <div style={{ padding:"8px 20px 0" }}>
      <p style={{ fontSize:11, fontWeight:600, letterSpacing:"2px", textTransform:"uppercase",
        color:"var(--gold)", marginBottom:14, opacity:.7 }}>Past Events</p>
      <div style={{ display:"grid", gridTemplateColumns:"1fr 1fr", gap:12 }}>
        {["🎉","📸","💃","🌹"].map((e,i) => (
          <div key={i} style={{ height:110, borderRadius:16,
            background:["linear-gradient(135deg,#1a1200,#3d2e00)","linear-gradient(135deg,#2e2000,#5a3e00)",
              "linear-gradient(135deg,#0a0804,#2a1f00)","linear-gradient(135deg,#1a1508,#3d2e00)"][i],
            display:"flex", alignItems:"center", justifyContent:"center",
            fontSize:40, border:"1px solid var(--border)" }}>{e}</div>
        ))}
      </div>
    </div>
  </div>
);

// ── RSVP ──────────────────────────────────────────────────────────────────────
const RSVPPage = ({ event }) => {
  const [form, setForm] = useState({ name:"", email:"", question:"" });
  const [status, setStatus] = useState(null);
  const ev = event || events[0];
  const submit = () => { if (!form.name || !form.email) return; setStatus(Math.random()>.4?"approved":"waiting"); };

  if (status) return (
    <div style={{ display:"flex", flexDirection:"column", alignItems:"center",
      justifyContent:"center", minHeight:700, padding:32, textAlign:"center" }}>
      <div style={{ fontSize:72, marginBottom:20 }}>{status==="approved"?"🎉":"⏳"}</div>
      <h2 className="serif" style={{ fontSize:28, marginBottom:12,
        background:"linear-gradient(135deg,#F0C060,#C9974A)",
        WebkitBackgroundClip:"text", WebkitTextFillColor:"transparent" }}>
        {status==="approved"?"You're in!":"You're on the list!"}
      </h2>
      <p style={{ color:"var(--muted)", lineHeight:1.6, maxWidth:280 }}>
        {status==="approved"
          ?`Your spot is confirmed. We can't wait to see you at ${ev.name}! ✦`
          :"Your request is under review. We'll notify you soon via email."}
      </p>
      <div style={{ marginTop:24, padding:"16px 24px", background:"var(--surface)",
        borderRadius:16, border:"1px solid var(--border)" }}>
        <div style={{ fontSize:13, fontWeight:600, color:"var(--gold)" }}>{ev.name}</div>
        <div style={{ fontSize:12, color:"var(--muted)", marginTop:4 }}>{ev.date} · {ev.place}</div>
      </div>
      <button className="btn-outline" style={{ marginTop:24 }} onClick={() => setStatus(null)}>← Back</button>
    </div>
  );

  return (
    <div>
      <div style={{ background:"linear-gradient(160deg,#1a1200,#2e2000)",
        borderBottom:"1px solid var(--border)", padding:"40px 28px 32px", marginBottom:24 }}>
        <div style={{ fontSize:40, marginBottom:12 }}>{ev.emoji||"🌸"}</div>
        <h2 className="serif" style={{ fontSize:26, marginBottom:8,
          background:"linear-gradient(135deg,#fff,#F0C060)",
          WebkitBackgroundClip:"text", WebkitTextFillColor:"transparent" }}>{ev.name}</h2>
        <div style={{ color:"var(--muted)", fontSize:13 }}>📅 {ev.date} &nbsp;·&nbsp; 📍 {ev.place}</div>
      </div>
      <div style={{ padding:"0 20px" }}>
        <p style={{ fontSize:11, fontWeight:600, letterSpacing:"2px", textTransform:"uppercase",
          color:"var(--gold)", marginBottom:20, opacity:.7 }}>Reserve Your Spot</p>
        <div style={{ display:"flex", flexDirection:"column", gap:16 }}>
          <div><label>Full Name *</label>
            <input placeholder="Your name" value={form.name} onChange={e=>setForm(p=>({...p,name:e.target.value}))}/></div>
          <div><label>Email *</label>
            <input type="email" placeholder="you@email.com" value={form.email} onChange={e=>setForm(p=>({...p,email:e.target.value}))}/></div>
          <div><label>Why do you want to attend? (optional)</label>
            <textarea rows={3} placeholder="Tell us a little about yourself…" value={form.question}
              onChange={e=>setForm(p=>({...p,question:e.target.value}))}/></div>
          <button className="btn-gold" style={{ width:"100%", marginTop:4 }} onClick={submit}>
            Confirm My Spot ✦
          </button>
        </div>
      </div>
    </div>
  );
};

// ── PROFILE ───────────────────────────────────────────────────────────────────
const ProfilePage = ({ onLogout }) => {
  const [notifs, setNotifs] = useState(true);
  const [editing, setEditing] = useState(false);
  const [profile, setProfile] = useState({
    name:"Aanya Sharma", email:"aanya@email.com",
    bio:"Founder · Mumbai · Passionate about women's empowerment ✦"
  });

  return (
    <div>
      <div style={{ background:"radial-gradient(ellipse at 50% 0%,#2a1f00,#0a0804)",
        padding:"60px 28px 40px", textAlign:"center", borderBottom:"1px solid var(--border)" }}>
        <div style={{ width:84, height:84, borderRadius:"50%", background:"linear-gradient(135deg,#1a1508,#2e2000)",
          display:"flex", alignItems:"center", justifyContent:"center",
          fontSize:36, margin:"0 auto 12px", border:"2px solid var(--gold)",
          boxShadow:"0 0 24px rgba(201,151,74,.3)" }}>🌸</div>
        {editing ? (
          <div style={{ display:"flex", flexDirection:"column", gap:10, marginTop:8 }}>
            <input value={profile.name} onChange={e=>setProfile(p=>({...p,name:e.target.value}))} style={{ textAlign:"center" }}/>
            <textarea rows={2} value={profile.bio} onChange={e=>setProfile(p=>({...p,bio:e.target.value}))} style={{ textAlign:"center", fontSize:12 }}/>
            <button className="btn-gold" onClick={()=>setEditing(false)}>Save Changes</button>
          </div>
        ) : (
          <>
            <h3 className="serif" style={{ fontSize:22, marginBottom:4,
              background:"linear-gradient(135deg,#fff,#F0C060)",
              WebkitBackgroundClip:"text", WebkitTextFillColor:"transparent" }}>{profile.name}</h3>
            <div style={{ color:"var(--muted)", fontSize:13, marginBottom:6 }}>{profile.email}</div>
            <div style={{ color:"rgba(201,151,74,.7)", fontSize:12, lineHeight:1.5,
              maxWidth:260, margin:"0 auto" }}>{profile.bio}</div>
            <button className="btn-outline" style={{ marginTop:16, fontSize:12, padding:"8px 20px" }}
              onClick={()=>setEditing(true)}>Edit Profile</button>
          </>
        )}
      </div>

      <div style={{ padding:"24px 20px 12px" }}>
        <p style={{ fontSize:11, fontWeight:600, letterSpacing:"2px", textTransform:"uppercase",
          color:"var(--gold)", marginBottom:14, opacity:.7 }}>My Events</p>
        {[events[0],events[2]].map(e => (
          <div key={e.id} style={{ display:"flex", alignItems:"center", gap:14,
            padding:"14px 16px", background:"var(--card)", borderRadius:14,
            marginBottom:10, border:"1px solid var(--border)" }}>
            <div style={{ width:44, height:44, borderRadius:12, background:e.bg,
              display:"flex", alignItems:"center", justifyContent:"center",
              fontSize:22, flexShrink:0, border:"1px solid var(--border)" }}>{e.emoji}</div>
            <div style={{ flex:1 }}>
              <div style={{ fontSize:14, fontWeight:600, color:"var(--text)" }}>{e.name}</div>
              <div style={{ fontSize:11, color:"var(--muted)" }}>{e.date}</div>
            </div>
            <span className="tag">Going</span>
          </div>
        ))}
      </div>

      <div style={{ margin:"8px 0" }}>
        {[["Event Notifications","New events & reminders",notifs,()=>setNotifs(n=>!n)],
          ["Community Updates","Announcements & news",true,null]].map(([title,sub,on,toggle],i) => (
          <div key={i} className="settings-row">
            <div>
              <div style={{ fontSize:14, fontWeight:500, color:"var(--text)" }}>{title}</div>
              <div style={{ fontSize:11, color:"var(--muted)" }}>{sub}</div>
            </div>
            <button className={`toggle ${on?"on":"off"}`} onClick={toggle||undefined}
              style={!toggle?{cursor:"default"}:{}}/>
          </div>
        ))}
      </div>

      <div style={{ padding:"20px" }}>
        <button onClick={onLogout} style={{ width:"100%", padding:"14px",
          background:"transparent", border:"1.5px solid rgba(201,151,74,.3)", borderRadius:14,
          color:"var(--gold)", fontFamily:"'DM Sans',sans-serif", fontSize:14,
          fontWeight:500, cursor:"pointer" }}>Log Out</button>
      </div>
    </div>
  );
};

// ── ROOT ──────────────────────────────────────────────────────────────────────
export default function App() {
  const [phase, setPhase] = useState("popup");
  const [tab, setTab]     = useState("home");
  const [rsvpEvent, setRsvpEvent] = useState(null);

  const tabs = [
    { id:"home",     label:"Home",    icon:"home" },
    { id:"announce", label:"Events",  icon:"announce" },
    { id:"rsvp",     label:"Book",    icon:"book" },
    { id:"profile",  label:"Profile", icon:"profile" },
  ];

  const goRSVP = ev => { setRsvpEvent(ev||null); setTab("rsvp"); };

  return (
    <>
      <GlobalStyle/>
      <div style={{ background:"#050403", minHeight:"100vh", padding:"0 0 40px" }}>
        <div className="shell">
          {phase==="popup"  && <LogoPopup onDone={()=>setPhase("auth")}/>}
          {phase==="auth"   && <AuthScreen onAuth={()=>setPhase("app")}/>}
          {phase==="app"    && (
            <>
              <div className="screen">
                {tab==="home"     && <HomePage onRSVP={goRSVP}/>}
                {tab==="announce" && <AnnouncementPage onRSVP={goRSVP}/>}
                {tab==="rsvp"     && <RSVPPage event={rsvpEvent}/>}
                {tab==="profile"  && <ProfilePage onLogout={()=>setPhase("auth")}/>}
              </div>
              <nav className="nav">
                {tabs.map(t => (
                  <button key={t.id} className={`nav-btn ${tab===t.id?"active":""}`}
                    onClick={()=>setTab(t.id)}>
                    <Icon name={t.icon}/>{t.label}
                  </button>
                ))}
              </nav>
            </>
          )}
        </div>
      </div>
    </>
  );
}
