```aura width=860 height=460 link="[https://collectioneur.github.io/readme-aura/](https://collectioneur.github.io/readme-aura/)"
<div style={{
  display: 'flex', flexDirection: 'column', width: '100%', height: '100%',
  background: '#030305', borderRadius: 24, border: '1px solid rgba(255,255,255,0.06)',
  position: 'relative', overflow: 'hidden', fontFamily: 'Inter, sans-serif'
}}>

  <svg width="860" height="460" style={{ position: 'absolute', top: 0, left: 0, opacity: 0.85 }}>
    <defs>
      <radialGradient id="glow-top" cx="30%" cy="0%" r="60%">
        <stop offset="0%" stopColor="rgba(0, 255, 204, 0.15)" />
        <stop offset="100%" stopColor="rgba(0, 255, 204, 0)" />
      </radialGradient>
      <radialGradient id="glow-bottom" cx="80%" cy="100%" r="60%">
        <stop offset="0%" stopColor="rgba(110, 80, 255, 0.15)" />
        <stop offset="100%" stopColor="rgba(110, 80, 255, 0)" />
      </radialGradient>
    </defs>
    <rect width="860" height="460" fill="url(#glow-top)" />
    <rect width="860" height="460" fill="url(#glow-bottom)" />


    <pattern id="grid" width="30" height="30" patternUnits="userSpaceOnUse">
      <path d="M 30 0 L 0 0 0 30" fill="none" stroke="rgba(255,255,255,0.02)" strokeWidth="1"/>
    </pattern>
    <rect width="860" height="460" fill="url(#grid)" />
  </svg>

  {/* --- HEADER SECTION --- */}
  <div style={{ display: 'flex', width: '100%', padding: '40px 40px 20px 40px', alignItems: 'center', zIndex: 10 }}>
    <div style={{
      width: 100, height: 100, borderRadius: 50, background: 'rgba(255,255,255,0.02)',
      border: '1px solid rgba(255,255,255,0.1)', display: 'flex', alignItems: 'center', justifyContent: 'center',
      boxShadow: '0 10px 30px rgba(0,0,0,0.5)'
    }}>
      <img src={github?.user?.avatarUrl ?? '[https://github.com/beellionaire.png](https://github.com/beellionaire.png)'} width={88} height={88} style={{ borderRadius: 44 }} />
    </div>

    <div style={{ display: 'flex', flexDirection: 'column', marginLeft: 28, justifyContent: 'center' }}>
      <div style={{ display: 'flex', color: '#00ffcc', fontSize: 12, letterSpacing: '3px', fontWeight: 600, textTransform: 'uppercase', marginBottom: 4 }}>
        Software Engineer • UI/UX Designer
      </div>
      <div style={{ display: 'flex', color: '#ffffff', fontSize: 42, fontWeight: 800, letterSpacing: '-1.5px', lineHeight: 1 }}>
        nabil abiyu.
      </div>
    </div>


    <div style={{ display: 'flex', marginLeft: 'auto', padding: '8px 16px', borderRadius: 20, background: 'rgba(0,255,204,0.05)', border: '1px solid rgba(0,255,204,0.2)', alignItems: 'center', gap: 8 }}>
      <div style={{ width: 8, height: 8, borderRadius: 4, background: '#00ffcc' }}></div>
      <span style={{ color: '#00ffcc', fontSize: 11, fontWeight: 600, letterSpacing: '1px' }}>AVAILABLE FOR COLLAB</span>
    </div>
  </div>


  <div style={{ display: 'flex', width: '100%', padding: '0 40px', gap: 16, zIndex: 10, marginTop: 10 }}>


    <div style={{ display: 'flex', flex: 1.2, flexDirection: 'column', background: 'rgba(255,255,255,0.02)', borderRadius: 16, border: '1px solid rgba(255,255,255,0.05)', padding: 24 }}>
      <div style={{ display: 'flex', color: 'rgba(255,255,255,0.4)', fontSize: 10, letterSpacing: '2px', fontWeight: 600, marginBottom: 12 }}>
        CURRENT INITIATIVES
      </div>
      <div style={{ display: 'flex', color: '#e6edf3', fontSize: 14, lineHeight: 1.6, fontWeight: 400 }}>
        Architecting robust full-stack web ecosystems and localized fintech trading tools. Focused on seamless Telegram Webhook automations and delivering pixel-perfect, intuitive user interfaces.
      </div>
      <div style={{ display: 'flex', gap: 8, marginTop: 'auto', flexWrap: 'wrap' }}>
         <div style={{ display: 'flex', padding: '4px 12px', borderRadius: 12, background: 'rgba(255,255,255,0.03)', border: '1px solid rgba(255,255,255,0.08)', color: '#8b949e', fontSize: 10, fontWeight: 500 }}>Fintech Solutions</div>
         <div style={{ display: 'flex', padding: '4px 12px', borderRadius: 12, background: 'rgba(255,255,255,0.03)', border: '1px solid rgba(255,255,255,0.08)', color: '#8b949e', fontSize: 10, fontWeight: 500 }}>API Integrations</div>
      </div>
    </div>


    <div style={{ display: 'flex', flex: 1, flexDirection: 'column', background: 'rgba(255,255,255,0.02)', borderRadius: 16, border: '1px solid rgba(255,255,255,0.05)', padding: 24 }}>
      <div style={{ display: 'flex', color: 'rgba(255,255,255,0.4)', fontSize: 10, letterSpacing: '2px', fontWeight: 600, marginBottom: 16 }}>
        CORE ARSENAL
      </div>
      <div style={{ display: 'flex', flexWrap: 'wrap', gap: 10 }}>
        {['Laravel', 'Next.js', 'React', 'Tailwind CSS', 'TypeScript', 'PHP', 'MySQL', 'Figma', 'Telegram API'].map((tag, i) => (
          <div key={i} style={{
            display: 'flex', padding: '6px 14px', borderRadius: 16,
            background: 'rgba(255,255,255,0.04)', border: '1px solid rgba(255,255,255,0.1)',
            color: '#c9d1d9', fontSize: 11, fontWeight: 500
          }}>
            {tag}
          </div>
        ))}
      </div>
    </div>
  </div>


  <div style={{ display: 'flex', width: '100%', padding: '0 40px', marginTop: 24, zIndex: 10, gap: 12, justifyContent: 'center' }}>
    {['GitHub', 'LinkedIn', 'Portfolio', 'Email'].map((social, i) => (
      <div key={i} style={{
        display: 'flex', padding: '8px 24px', borderRadius: 20,
        background: 'rgba(255,255,255,0.02)', border: '1px solid rgba(255,255,255,0.08)',
        color: 'rgba(255,255,255,0.6)', fontSize: 12, fontWeight: 500, letterSpacing: '0.5px'
      }}>
        {social}
      </div>
    ))}
  </div>
</div>
```

<br>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=beellionaire&show_icons=true&theme=transparent&hide_border=true&title_color=00ffcc&icon_color=6e50ff&text_color=8b949e&v=2" width="48%" alt="GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=beellionaire&layout=compact&theme=transparent&hide_border=true&title_color=00ffcc&text_color=8b949e&v=2" width="48%" alt="Top Languages" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=beellionaire&bg_color=transparent&color=00ffcc&line=6e50ff&point=ffffff&hide_border=true&v=2" width="100%" alt="Activity Graph" />
</p>
