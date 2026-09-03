```aura width=860 height=230 link="https://collectioneur.github.io/readme-aura/"
<div style={{
  width:'100%', height:'100%',
  background:'#07070b',
  display:'flex',
  alignItems:'center',
  fontFamily:'Inter',
  position:'relative',
  overflow:'hidden',
  borderRadius:18,
  border:'1px solid rgba(130,90,255,0.25)'
}}>

  <style>{`
    @keyframes drift {
      0%,100% { transform:translateX(0) translateY(0); opacity:.45; }
      50% { transform:translateX(120px) translateY(-25px); opacity:.8; }
    }

    @keyframes drift2 {
      0%,100% { transform:translateX(0); opacity:.3; }
      50% { transform:translateX(-140px); opacity:.65; }
    }

    @keyframes pulse {
      0%,100% { opacity:.25; }
      50% { opacity:.65; }
    }

    #orb1 { animation:drift 10s ease-in-out infinite; }
    #orb2 { animation:drift2 13s ease-in-out infinite; }
    #orb3 { animation:pulse 6s ease-in-out infinite; }

    .cursor {
      animation:pulse 1s steps(2) infinite;
    }
  `}</style>

  <!-- Background -->
  <svg width="860" height="230"
       style={{position:'absolute',top:0,left:0}}>

    <defs>

      <radialGradient id="purple">
        <stop offset="0%" stopColor="rgba(125,70,255,.45)" />
        <stop offset="100%" stopColor="rgba(125,70,255,0)" />
      </radialGradient>

      <radialGradient id="blue">
        <stop offset="0%" stopColor="rgba(30,120,255,.35)" />
        <stop offset="100%" stopColor="rgba(30,120,255,0)" />
      </radialGradient>

      <linearGradient id="line">
        <stop offset="0%" stopColor="rgba(130,90,255,0)" />
        <stop offset="50%" stopColor="rgba(130,90,255,.35)" />
        <stop offset="100%" stopColor="rgba(130,90,255,0)" />
      </linearGradient>

    </defs>

    <ellipse
      id="orb1"
      cx="160"
      cy="210"
      rx="260"
      ry="150"
      fill="url(#purple)"
    />

    <ellipse
      id="orb2"
      cx="720"
      cy="40"
      rx="230"
      ry="150"
      fill="url(#blue)"
    />

    <ellipse
      id="orb3"
      cx="500"
      cy="180"
      rx="170"
      ry="100"
      fill="url(#purple)"
    />

    <rect
      x="0"
      y="188"
      width="860"
      height="1"
      fill="url(#line)"
    />

  </svg>

  <!-- Avatar -->
  <div style={{
    position:'absolute',
    left:42,
    top:65,
    width:100,
    height:100,
    borderRadius:50,
    background:'linear-gradient(135deg,#7c3aed,#2563eb)',
    display:'flex',
    alignItems:'center',
    justifyContent:'center',
    boxShadow:'0 0 35px rgba(100,60,255,.35)'
  }}>

    <img
      src={github?.user?.avatarUrl ?? 'https://github.com/adria296.png'}
      width={92}
      height={92}
      style={{borderRadius:46}}
    />

  </div>

  <!-- Content -->
  <div style={{
    display:'flex',
    flexDirection:'column',
    marginLeft:168,
    gap:9,
    zIndex:10
  }}>

    <div style={{
      display:'flex',
      fontSize:36,
      fontWeight:800,
      color:'#ffffff',
      letterSpacing:'-1px'
    }}>
      Adrian Dorado
    </div>

    <div style={{
      display:'flex',
      fontSize:15,
      color:'rgba(190,180,230,.75)',
      letterSpacing:'.2px'
    }}>
      BSIT Student • Aspiring Software & Web Developer
    </div>

    <div style={{
      display:'flex',
      alignItems:'center',
      gap:7,
      marginTop:3,
      fontSize:13,
      color:'rgba(150,130,220,.85)'
    }}>
      <span style={{color:'#8b5cf6'}}>&gt;</span>
      <span>building • learning • improving</span>
      <span class="cursor" style={{color:'#8b5cf6'}}>▌</span>
    </div>

    <div style={{
      display:'flex',
      gap:7,
      marginTop:4,
      flexWrap:'wrap'
    }}>

      {[
        'JavaScript',
        'C',
        'Node.js',
        'Frontend'
      ].map(function(tag, i) {

        return (
          <div key={tag + i} style={{
            display:'flex',
            padding:'5px 11px',
            borderRadius:8,
            background:'rgba(120,80,255,.10)',
            border:'1px solid rgba(130,90,255,.25)',
            color:'rgba(215,205,255,.85)',
            fontSize:11,
            fontWeight:600
          }}>
            {tag}
          </div>
        );

      })}

    </div>

  </div>

  <!-- Small status -->
  <div style={{
    position:'absolute',
    right:24,
    bottom:17,
    display:'flex',
    alignItems:'center',
    gap:7,
    fontSize:10,
    color:'rgba(170,160,200,.45)'
  }}>
    <div style={{
      width:6,
      height:6,
      borderRadius:3,
      background:'#7c3aed'
    }} />
    learning mode
  </div>

</div>
```

```aura width=860 height=28 link="https://collectioneur.github.io/readme-aura/"
<div style={{
  display:'flex',
  justifyContent:'center',
  alignItems:'center',
  width:'100%',
  height:'100%',
  fontFamily:'Inter',
  fontSize:11,
  color:'rgba(150,140,190,.45)',
  letterSpacing:'.6px'
}}>
  <span>crafted by adria296 • powered by readme-aura</span>
</div>
```

````

### What I changed

- **Adrian Dorado** instead of `repo?.name`
- Your actual developer direction: **Software & Web Developer**
- Your current technologies: **JavaScript, C, Node.js, Frontend**
- Added a little terminal-style `>` effect
- Added a subtle animated cursor
- Purple/blue glow instead of the common huge rainbow blobs
- Added a small **"learning mode"** status
- Cleaner rounded cards and less visual clutter
- Your GitHub avatar automatically loads from `github.com/adria296.png`

After replacing `readme.source.md`, run:

```bash
npx readme-aura build
````

Then open your generated `README.md` to preview it.

If you like it, **then** we'll commit and push it to GitHub.
