<div style={{
  width: '100%', height: '100%', background: '#09090b', // Deep minimalist black
  display: 'flex', alignItems: 'center', fontFamily: 'Inter, sans-serif',
  position: 'relative', overflow: 'hidden', borderRadius: 16,
  border: '1px solid rgba(255,255,255,0.08)' // Subtle glass edge
}}>

  <style>{`
    /* Animasi yang lebih lambat dan elegan (Ambient Flow) */
    @keyframes ambient-drift {
      0%, 100% { transform: translate(0, 0) scale(1); opacity: 0.6; }
      50% { transform: translate(40px, -20px) scale(1.1); opacity: 0.9; }
    }
    @keyframes ambient-pulse {
      0%, 100% { transform: translate(0, 0) scale(1); opacity: 0.5; }
      50% { transform: translate(-30px, 20px) scale(1.2); opacity: 0.8; }
    }
    #glow-cyan { animation: ambient-drift 12s ease-in-out infinite; }
    #glow-blue { animation: ambient-pulse 15s ease-in-out infinite; }
    #glow-violet { animation: ambient-drift 18s ease-in-out infinite reverse; }
  `}</style>

{/\_ Latar Belakang Aura Minimalis \_/} \<svg width="860" height="200" style={{ position: 'absolute', top: 0, left: 0, opacity: 0.8 }}> <defs> <radialGradient id="grad-cyan" cx="50%" cy="50%" r="50%"> <stop offset="0%" stopColor="rgba(0, 255, 204, 0.20)" /> <stop offset="50%" stopColor="rgba(0, 255, 204, 0.05)" /> <stop offset="100%" stopColor="rgba(0, 255, 204, 0)" /> </radialGradient> <radialGradient id="grad-blue" cx="50%" cy="50%" r="50%"> <stop offset="0%" stopColor="rgba(0, 119, 255, 0.25)" /> <stop offset="50%" stopColor="rgba(0, 119, 255, 0.08)" /> <stop offset="100%" stopColor="rgba(0, 119, 255, 0)" /> </radialGradient> <radialGradient id="grad-violet" cx="50%" cy="50%" r="50%"> <stop offset="0%" stopColor="rgba(139, 92, 246, 0.15)" /> <stop offset="50%" stopColor="rgba(139, 92, 246, 0.05)" /> <stop offset="100%" stopColor="rgba(139, 92, 246, 0)" /> </radialGradient> </defs>

```
<ellipse id="glow-cyan" cx="200" cy="100" rx="300" ry="200" fill="url(#grad-cyan)" />
<ellipse id="glow-blue" cx="600" cy="150" rx="400" ry="250" fill="url(#grad-blue)" />
<ellipse id="glow-violet" cx="400" cy="0" rx="350" ry="200" fill="url(#grad-violet)" />
```

  </svg>

{/\_ Pattern Grid Transparan (Memberikan tekstur "Tech" yang mewah) \_/}

  <div style={{
    position: 'absolute', top: 0, left: 0, right: 0, bottom: 0,
    backgroundImage: 'linear-gradient(rgba(255,255,255,0.02) 1px, transparent 1px), linear-gradient(90deg, rgba(255,255,255,0.02) 1px, transparent 1px)',
    backgroundSize: '20px 20px',
    opacity: 1, zIndex: 1
  }}></div>

{/\_ Konten Utama \_/}

  <div style={{ display: 'flex', alignItems: 'center', width: '100%', padding: '0 45px', zIndex: 10 }}>

```
{/* Avatar Frame (Gaya Glassmorphism) */}
<div style={{
  width: 110, height: 110, borderRadius: 55,
  background: 'rgba(255,255,255,0.03)',
  border: '1px solid rgba(255,255,255,0.15)',
  display: 'flex', alignItems: 'center', justifyContent: 'center',
  boxShadow: '0 8px 32px rgba(0,0,0,0.3)',
}}>
  <img src={github?.user?.avatarUrl ?? 'https://github.com/beellionaire.png'} width={94} height={94} style={{ borderRadius: 47 }} />
</div>

{/* Teks & Lencana Bahasa */}
<div style={{ display:'flex', flexDirection:'column', marginLeft: 35, gap: 4 }}>

  <div style={{ display:'flex', fontSize: 11, fontWeight: 600, color: '#00ffcc', letterSpacing: '2px', textTransform: 'uppercase', marginBottom: 2 }}>
    Software Engineer • UI/UX Designer
  </div>

  <div style={{ display:'flex', fontSize: 40, fontWeight: 800, color: '#ffffff', letterSpacing: '-1px', lineHeight: 1.1 }}>
    {github?.user?.name || github?.user?.login || 'Nabil Abiyu'}
  </div>

  <div style={{ display:'flex', fontSize: 14, color: '#8b949e', fontWeight: 400, letterSpacing: '0.3px', maxWidth: 550, marginTop: 4 }}>
    {github?.user?.bio || 'Building scalable architectures and designing intuitive digital experiences from Indonesia.'}
  </div>

  <div style={{ display:'flex', gap: 10, marginTop: 14, flexWrap: 'wrap' }}>
    {((github && github.languages && github.languages.length > 0)
      ? github.languages.slice(0, 5).map(function(l) { return l.name; })
      : ['Laravel', 'Next.js', 'React', 'TypeScript', 'Tailwind']
    ).map(function(tag, i) {
      return (
        <div key={tag + '-' + i} style={{
          display:'flex', padding:'5px 14px', borderRadius: 4, // Ujung sedikit kotak agar terlihat modern
          background:'rgba(255,255,255,0.04)', border:'1px solid rgba(255,255,255,0.12)',
          color:'#c9d1d9', fontSize: 10, fontWeight: 600, letterSpacing: '1px', textTransform: 'uppercase'
        }}>{tag}</div>
      );
    })}
  </div>
</div>
```

  </div>
</div>
