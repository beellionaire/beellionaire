```aura width=860 height=480 link="[https://collectioneur.github.io/readme-aura/](https://collectioneur.github.io/readme-aura/)"
<div style={{
  display: 'flex', flexDirection: 'column', width: '100%', height: '100%',
  background: '#0a0a0a', borderRadius: 28, border: '1px solid rgba(255,255,255,0.06)',
  position: 'relative', overflow: 'hidden', fontFamily: 'Inter, sans-serif'
}}>

  {/* SVG Background Layer */}
  <svg width="100%" height="100%" style={{ position: 'absolute', top: 0, left: 0, opacity: 1, zIndex: 0 }}>
    <defs>
      <radialGradient id="aurora-teal" cx="20%" cy="100%" r="70%">
        <stop offset="0%" stopColor="rgba(42, 157, 143, 0.25)" />
        <stop offset="100%" stopColor="rgba(42, 157, 143, 0)" />
      </radialGradient>
      <radialGradient id="aurora-purple" cx="80%" cy="0%" r="70%">
        <stop offset="0%" stopColor="rgba(110, 80, 255, 0.25)" />
        <stop offset="100%" stopColor="rgba(110, 80, 255, 0)" />
      </radialGradient>
    </defs>
    <rect width="100%" height="100%" fill="url(#aurora-teal)" />
    <rect width="100%" height="100%" fill="url(#aurora-purple)" />
    <pattern id="dotpattern" width="30" height="30" patternUnits="userSpaceOnUse">
      <circle cx="2" cy="2" r="1" fill="rgba(255,255,255,0.03)"/>
    </pattern>
    <rect width="100%" height="100%" fill="url(#dotpattern)" />
  </svg>

  <div style={{ display: 'flex', flexDirection: 'column', width: '100%', height: '100%', padding: '50px', zIndex: 10 }}>

    {/* Header & Logo Section */}
    <div style={{ display: 'flex', alignItems: 'center', marginBottom: 40 }}>
      <div style={{ width: 80, height: 80, borderRadius: 20, background: 'rgba(255,255,255,0.02)', border: '1px solid rgba(255,255,255,0.1)', display: 'flex', alignItems: 'center', justifyContent: 'center' }}>
        <img src="https://github.com/github.png" width={60} height={60} />
      </div>
      <div style={{ display: 'flex', flexDirection: 'column', marginLeft: 30 }}>
        <div style={{ color: 'rgba(255,255,255,0.4)', fontSize: 13, letterSpacing: '6px', fontWeight: 600, textTransform: 'uppercase', marginBottom: 8 }}>
          Designer • Developer • Creator
        </div>
        <div style={{ color: '#ffffff', fontSize: 48, fontWeight: 900, letterSpacing: '-1.5px', lineHeight: 1 }}>
          nama profil kamu
        </div>
      </div>
    </div>

    {/* Content Grid */}
    <div style={{ display: 'flex', width: '100%', gap: 20 }}>

      {/* Main Glassmorphism Card */}
      <div style={{ display: 'flex', flex: 2, background: 'rgba(255,255,255,0.03)', borderRadius: 24, border: '1px solid rgba(255,255,255,0.06)', padding: 35, flexDirection: 'column', justifyContent: 'space-between' }}>
        <div>
          <div style={{ color: 'rgba(255,255,255,0.5)', fontSize: 11, letterSpacing: '4px', fontWeight: 600, textTransform: 'uppercase', marginBottom: 15 }}>
            About
          </div>
          <div style={{ color: '#c9d1d9', fontSize: 28, fontWeight: 700, letterSpacing: '0px', lineHeight: 1.2, maxWidth: '90%' }}>
            Membangun solusi digital yang estetis dan fungsional.
          </div>
        </div>
        <div style={{ display: 'flex', color: '#2a9d8f', fontSize: 14, letterSpacing: '0.5px', marginTop: 30, alignItems: 'center', gap: 10 }}>
          <span>> terbuka untuk kolaborasi</span>
        </div>
      </div>

      {/* Sidebar Mini Cards */}
      <div style={{ display: 'flex', flex: 1, flexDirection: 'column', gap: 20 }}>
        <div style={{ display: 'flex', flex: 1, background: 'rgba(255,255,255,0.03)', borderRadius: 20, border: '1px solid rgba(255,255,255,0.06)', padding: '20px 24px', flexDirection: 'column', justifyContent: 'center' }}>
          <div style={{ color: 'rgba(255,255,255,0.3)', fontSize: 10, letterSpacing: '3px', fontWeight: 600, textTransform: 'uppercase', marginBottom: 10 }}>
            Fokus Utama
          </div>
          <div style={{ color: '#fff', fontSize: 13, fontWeight: 500, letterSpacing: '1px' }}>
            ◆ UI/UX. ◆ FRONTEND. ◆ SVG.
          </div>
        </div>
        <div style={{ display: 'flex', flex: 1, background: 'rgba(2a,9d,8f,0.06)', borderRadius: 20, border: '1px solid rgba(2a,9d,8f,0.2)', padding: '20px 24px', alignItems: 'center', justifyContent: 'center' }}>
          <div style={{ color: '#fff', fontSize: 13, fontWeight: 500, letterSpacing: '1px' }}>
            Cek portofolio terbaru saya →
          </div>
        </div>
      </div>
    </div>

    {/* Contact & Tech Stack Footer */}
    <div style={{ display: 'flex', justifyContent: 'center', alignItems: 'center', width: '100%', marginTop: 'auto', borderTop: '1px solid rgba(255,255,255,0.04)', paddingTop: 16 }}>
      <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.3)', fontWeight: 500, letterSpacing: '3px', textTransform: 'uppercase' }}>crafted with precision • driven by logic</span>
    </div>

  </div>
</div>
```
