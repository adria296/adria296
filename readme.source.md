```aura width=860 height=200

  <div style={{

 width: '100%', height: '100%', background: '#08080c',

 display: 'flex', alignItems: 'center', fontFamily: 'Inter',

 position: 'relative', overflow: 'hidden', borderRadius: 16,

 border: '1px solid rgba(220,38,38,0.18)'

}}>

 <style>

   {`

     @keyframes float-slow {

       0%, 100% { transform: translateX(0px); opacity: 0.8; }

       50% { transform: translateX(350px); opacity: 1.2; }

     }

     @keyframes float-medium {

       0%, 100% { transform: translateX(0px); opacity: 0.7; }

       50% { transform: translateX(-250px); opacity: 1.1; }

     }

     @keyframes float-fast {

       0%, 100% { transform: translateX(0px); opacity: 0.9; }

       50% { transform: translateX(200px); opacity: 0.6; }

     }

     @keyframes float-diagonal {

       0%, 100% { transform: translateX(0px); opacity: 0.75; }

       50% { transform: translateX(300px); opacity: 1.0; }

     }

     @keyframes float-wave {

       0%, 100% { transform: translateX(0px); opacity: 0.65; }

       33% { transform: translateX(-160px); opacity: 0.9; }

       66% { transform: translateX(80px); opacity: 1.0; }

     }

     @keyframes float-pulse {

       0%, 100% { transform: scale(1); opacity: 0.8; }

       50% { transform: scale(1.3); opacity: 0.4; }

     }

     #glow-1 { animation: float-slow 8s ease-in-out infinite; }

     #glow-2 { animation: float-medium 12s ease-in-out infinite; }

     #glow-3 { animation: float-fast 9s ease-in-out infinite; }

     #glow-4 { animation: float-slow 11s ease-in-out infinite reverse; }

     #glow-5 { animation: float-medium 14s ease-in-out infinite reverse; }

     #glow-6 { animation: float-diagonal 10s ease-in-out infinite; }

     #glow-7 { animation: float-wave 13s ease-in-out infinite; }

     #glow-8 { animation: float-pulse 7s ease-in-out infinite; }

   `}

 </style>

 <svg width="860" height="200" style={{ position: 'absolute', top: 0, left: 0 }}>

   <defs>

     <radialGradient id="g1" cx="50%" cy="50%" r="50%">

       <stop offset="0%" stopColor="rgba(210, 20, 20, 0.72)" />

       <stop offset="40%" stopColor="rgba(180, 15, 15, 0.35)" />

       <stop offset="70%" stopColor="rgba(180,15,15,0)" />

     </radialGradient>

     <radialGradient id="g2" cx="50%" cy="50%" r="50%">

       <stop offset="0%" stopColor="rgba(255, 40, 40, 0.6)" />

       <stop offset="45%" stopColor="rgba(200, 30, 30, 0.25)" />

       <stop offset="70%" stopColor="rgba(200, 30, 30, 0)" />

     </radialGradient>

     <radialGradient id="g3" cx="50%" cy="50%" r="50%">

       <stop offset="0%" stopColor="rgba(255, 0, 0, 0.45)" />

       <stop offset="50%" stopColor="rgba(220, 0, 0, 0.18)" />

       <stop offset="70%" stopColor="rgba(220,0,0,0)" />

     </radialGradient>

     <radialGradient id="g4" cx="50%" cy="50%" r="50%">

       <stop offset="0%" stopColor="rgba(230, 0, 0, 0.32)" />

       <stop offset="70%" stopColor="rgba(230, 0, 0, 0)" />

     </radialGradient>

     <radialGradient id="g5" cx="50%" cy="50%" r="50%">

       <stop offset="0%" stopColor="rgba(200, 30, 30, 0.38)" />

       <stop offset="70%" stopColor="rgba(200, 30, 30, 0)" />

     </radialGradient>

     <radialGradient id="g6" cx="50%" cy="50%" r="50%">

       <stop offset="0%" stopColor="rgba(255, 30, 30, 0.55)" />

       <stop offset="45%" stopColor="rgba(220, 20, 20, 0.22)" />

       <stop offset="70%" stopColor="rgba(220,20,20,0)" />

     </radialGradient>

     <radialGradient id="g7" cx="50%" cy="50%" r="50%">

       <stop offset="0%" stopColor="rgba(255, 20, 20, 0.42)" />

       <stop offset="50%" stopColor="rgba(200, 10, 10, 0.16)" />

       <stop offset="70%" stopColor="rgba(200, 10, 10, 0)" />

     </radialGradient>

     <radialGradient id="g8" cx="50%" cy="50%" r="50%">

       <stop offset="0%" stopColor="rgba(255, 0, 0, 0.4)" />

       <stop offset="50%" stopColor="rgba(220,20,20,0.15)" />

       <stop offset="70%" stopColor="rgba(220,20,20,0)" />

     </radialGradient>

   </defs>

   <ellipse id="glow-1" cx="180" cy="230" rx="260" ry="190" fill="url(#g1)" />

   <ellipse id="glow-2" cx="300" cy="240" rx="220" ry="160" fill="url(#g2)" />

   <ellipse id="glow-3" cx="420" cy="240" rx="180" ry="140" fill="url(#g3)" />

   <ellipse id="glow-4" cx="550" cy="250" rx="150" ry="120" fill="url(#g4)" />

   <ellipse id="glow-5" cx="750" cy="250" rx="130" ry="110" fill="url(#g5)" />

   <ellipse id="glow-6" cx="300" cy="240" rx="180" ry="140" fill="url(#g6)" />

   <ellipse id="glow-7" cx="490" cy="230" rx="220" ry="170" fill="url(#g7)" />

   <ellipse id="glow-8" cx="590" cy="250" rx="150" ry="130" fill="url(#g8)" />

 </svg>

 <div style={{

   position: 'absolute', left: 48, top: 52, width: 96, height: 96,

   borderRadius: 48, background: 'linear-gradient(135deg, #dc2626, #ff3b30)',

   display: 'flex', alignItems: 'center', justifyContent: 'center',

 }}>

   <img src={(github && github.user && github.user.avatarUrl) || 'https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png'} width={88} height={88} style={{ borderRadius: 44 }} />

 </div>

 <div style={{ display:'flex', flexDirection:'column', marginLeft:168, gap:8, zIndex: 10 }}>

   <div style={{ display:'flex', fontSize:38, fontWeight:800, color:'#ffffff', letterSpacing:'-1px', lineHeight:1 }}>

     {(github && github.user && (github.user.name || github.user.login)) || 'GitHub Developer'}

   </div>

   <div style={{ display:'flex', fontSize:15, color:'rgba(255,180,180,0.8)', fontWeight:400, letterSpacing:'0.3px' }}>

     {(github && github.user && github.user.bio) || 'Developer · Competitive Programmer · Open Source'}

   </div>

   <div style={{ display:'flex', gap:8, marginTop:6 }}>

     {['HTML', 'CSS', 'JavaScript', 'C'].map(function(tag) {

       return (

         <div key={tag} style={{

           display:'flex', padding:'4px 12px', borderRadius:20,

           background:'rgba(220,38,38,0.18)', border:'1px solid rgba(220,38,38,0.32)',

           color:'rgba(255,220,220,0.85)', fontSize:12, fontWeight:600,

         }}>{tag}</div>

       );

     })}

   </div>

 </div>

</div>



(function() {

 var stats = [

   { label: 'Repos', value: String((github && github.stats && github.stats.totalRepos) || 0), color: '#ef4444' },

   { label: 'Stars', value: String((github && github.stats && github.stats.totalStars) || 0), color: '#f87171' },

   { label: 'Commits', value: String((github && github.stats && github.stats.totalCommits) || 0), color: '#fb7185' },

 ];

 return (

   <div style={{

     width: '100%', height: '100%',

     background: '#08080c',

     display: 'flex', alignItems: 'center', justifyContent: 'center',

     fontFamily: 'Inter', borderRadius: 16,

     border: '1px solid rgba(220,38,38,0.18)',

     position: 'relative', overflow: 'hidden',

   }}>

     <style>

       {`

         @keyframes float-slow {

           0%, 100% { transform: translateX(0px); opacity: 0.8; }

           50% { transform: translateX(350px); opacity: 1.2; }

         }

         @keyframes float-medium {

           0%, 100% { transform: translateX(0px); opacity: 0.7; }

           50% { transform: translateX(-250px); opacity: 1.1; }

         }

         @keyframes float-fast {

           0%, 100% { transform: translateX(0px); opacity: 0.9; }

           50% { transform: translateX(200px); opacity: 0.6; }

         }

         @keyframes float-diagonal {

           0%, 100% { transform: translate(0px, 0px); opacity: 0.75; }

           50% { transform: translate(120px, 30px); opacity: 1.0; }

         }

         @keyframes float-wave {

           0%, 100% { transform: translateX(0px); opacity: 0.65; }

           33% { transform: translateX(-160px); opacity: 0.9; }

           66% { transform: translateX(80px); opacity: 1.0; }

         }

         @keyframes float-pulse {

           0%, 100% { transform: scale(1); opacity: 0.8; }

           50% { transform: scale(1.3); opacity: 0.4; }

         }

         #glow-1 { animation: float-slow 8s ease-in-out infinite; }

         #glow-2 { animation: float-medium 12s ease-in-out infinite; }

         #glow-3 { animation: float-fast 9s ease-in-out infinite; }

         #glow-4 { animation: float-diagonal 10s ease-in-out infinite; }

         #glow-5 { animation: float-wave 14s ease-in-out infinite; }

       `}

     </style>

     <svg width="860" height="140" style={{ position: 'absolute', top: 0, left: 0 }}>

       <defs>

         <radialGradient id="g1" cx="50%" cy="50%" r="50%">

           <stop offset="0%" stopColor="rgba(210,20,20,0.65)" />

           <stop offset="45%" stopColor="rgba(180,15,15,0.28)" />

           <stop offset="70%" stopColor="rgba(180,15,15,0)" />

         </radialGradient>

         <radialGradient id="g2" cx="50%" cy="50%" r="50%">

           <stop offset="0%" stopColor="rgba(255,40,40,0.55)" />

           <stop offset="45%" stopColor="rgba(200,20,20,0.22)" />

           <stop offset="70%" stopColor="rgba(200,20,20,0)" />

         </radialGradient>

         <radialGradient id="g3" cx="50%" cy="50%" r="50%">

           <stop offset="0%" stopColor="rgba(255,40,40,0.42)" />

           <stop offset="70%" stopColor="rgba(255,40,40,0)" />

         </radialGradient>

         <radialGradient id="g4" cx="50%" cy="50%" r="50%">

           <stop offset="0%" stopColor="rgba(255,70,70,0.30)" />

           <stop offset="70%" stopColor="rgba(255,70,70,0)" />

         </radialGradient>

         <radialGradient id="g5" cx="50%" cy="50%" r="50%">

           <stop offset="0%" stopColor="rgba(200,25,25,0.40)" />

           <stop offset="70%" stopColor="rgba(200,25,25,0)" />

         </radialGradient>

       </defs>

       <ellipse id="glow-1" cx="710" cy="150" rx="210" ry="150" fill="url(#g1)" />

       <ellipse id="glow-2" cx="550" cy="140" rx="190" ry="140" fill="url(#g2)" />

       <ellipse id="glow-3" cx="400" cy="130" rx="170" ry="130" fill="url(#g3)" />

       <ellipse id="glow-4" cx="250" cy="140" rx="150" ry="120" fill="url(#g4)" />

       <ellipse id="glow-5" cx="100" cy="150" rx="130" ry="110" fill="url(#g5)" />

     </svg>

     {stats.map(function(s, i) {

       return (

         <div key={s.label} style={{

           flexGrow: 1, display: 'flex', flexDirection: 'column',

           alignItems: 'center', justifyContent: 'center',

           padding: '16px 8px',

           borderRight: i < stats.length - 1 ? '1px solid rgba(255,255,255,0.06)' : 'none',

           gap: 5,

         }}>

           <div style={{ display:'flex', fontSize:30, fontWeight:800, color:s.color, lineHeight:1 }}>

             {s.value}

           </div>

           <div style={{ display:'flex', fontSize:11, color:'rgba(225,195,195,0.45)', fontWeight:600, letterSpacing:'1.5px' }}>

             {s.label.toUpperCase()}

           </div>

         </div>

       );

     })}

   </div>

 );

})()



(function() {

 var topLangs = (github && github.languages && github.languages.length > 0 ? github.languages.slice(0, 6).map(function(l) { return l.name; }) : ['TypeScript', 'React', 'Next.js', 'C++', 'Go', 'Rust']);

 var categories = [

   { title: 'Languages', color: '#ef4444', items: topLangs },

   { title: 'Frameworks', color: '#f87171', items: ['React Native', 'React', 'Next.js'] },

 ];

 return (

   <div style={{

     width: '100%', height: '100%',

     background: '#08080c',

     display: 'flex', flexDirection: 'column',

     fontFamily: 'Inter', padding: '18px 32px', gap: 14,

     borderRadius: 16, border: '1px solid rgba(220,38,38,0.18)',

     position: 'relative', overflow: 'hidden',

   }}>

     <style>

       {`

         @keyframes float-slow {

           0%, 100% { transform: translateX(0px); opacity: 0.8; }

           50% { transform: translateX(350px); opacity: 1.2; }

         }

         @keyframes float-medium {

           0%, 100% { transform: translateX(0px); opacity: 0.7; }

           50% { transform: translateX(-250px); opacity: 1.1; }

         }

         @keyframes float-fast {

           0%, 100% { transform: translateX(0px); opacity: 0.9; }

           50% { transform: translateX(200px); opacity: 0.6; }

         }

         @keyframes float-diagonal {

           0%, 100% { transform: translate(0px, 0px); opacity: 0.75; }

           50% { transform: translate(120px, 30px); opacity: 1.0; }

         }

         @keyframes float-wave {

           0%, 100% { transform: translateX(0px); opacity: 0.65; }

           33% { transform: translateX(-160px); opacity: 0.9; }

           66% { transform: translateX(80px); opacity: 1.0; }

         }

         @keyframes float-pulse {

           0%, 100% { transform: scale(1); opacity: 0.8; }

           50% { transform: scale(1.3); opacity: 0.4; }

         }

         #glow-1 { animation: float-slow 9s ease-in-out infinite; }

         #glow-2 { animation: float-medium 12s ease-in-out infinite; }

         #glow-3 { animation: float-fast 8s ease-in-out infinite; }

         #glow-4 { animation: float-diagonal 11s ease-in-out infinite reverse; }

         #glow-5 { animation: float-wave 14s ease-in-out infinite reverse; }

         #glow-6 { animation: float-pulse 6s ease-in-out infinite; }

       `}

     </style>

     <svg width="860" height="168" style={{ position: 'absolute', top: 0, left: 0 }}>

       <defs>

         <radialGradient id="g1" cx="50%" cy="50%" r="50%">

           <stop offset="0%" stopColor="rgba(215, 20, 20, 0.68)" />

           <stop offset="42%" stopColor="rgba(175, 15, 15, 0.3)" />

           <stop offset="70%" stopColor="rgba(175, 15, 15, 0)" />

         </radialGradient>

         <radialGradient id="g2" cx="50%" cy="50%" r="50%">

           <stop offset="0%" stopColor="rgba(255, 55, 55, 0.55)" />

           <stop offset="45%" stopColor="rgba(210, 35, 35, 0.22)" />

           <stop offset="70%" stopColor="rgba(210,25,25,0)" />

         </radialGradient>

         <radialGradient id="g3" cx="50%" cy="50%" r="50%">

           <stop offset="0%" stopColor="rgba(255, 0, 0, 0.42)" />

           <stop offset="50%" stopColor="rgba(220, 0, 0, 0.16)" />

           <stop offset="70%" stopColor="rgba(220, 0, 0, 0)" />

         </radialGradient>

         <radialGradient id="g4" cx="50%" cy="50%" r="50%">

           <stop offset="0%" stopColor="rgba(240, 0, 0, 0.32)" />

           <stop offset="70%" stopColor="rgba(240,0,0,0)" />

         </radialGradient>

         <radialGradient id="g5" cx="50%" cy="50%" r="50%">

           <stop offset="0%" stopColor="rgba(205, 25, 25, 0.42)" />

           <stop offset="70%" stopColor="rgba(205,25,25,0)" />

         </radialGradient>

         <radialGradient id="g6" cx="50%" cy="50%" r="50%">

           <stop offset="0%" stopColor="rgba(255, 60, 60, 0.35)" />

           <stop offset="70%" stopColor="rgba(255,50,50,0)" />

         </radialGradient>

       </defs>

       <ellipse id="glow-1" cx="170" cy="168" rx="260" ry="170" fill="url(#g1)" />

       <ellipse id="glow-2" cx="320" cy="178" rx="220" ry="140" fill="url(#g2)" />

       <ellipse id="glow-3" cx="460" cy="178" rx="190" ry="130" fill="url(#g3)" />

       <ellipse id="glow-4" cx="590" cy="188" rx="160" ry="110" fill="url(#g4)" />

       <ellipse id="glow-5" cx="750" cy="188" rx="140" ry="100" fill="url(#g5)" />

       <ellipse id="glow-6" cx="420" cy="138" rx="100" ry="80" fill="url(#g6)" />

     </svg>

     <div style={{ display:'flex', fontSize:10, fontWeight:700, color:'rgba(220,150,150,0.5)', letterSpacing:'3px' }}>

       TECH STACK

     </div>

     <div style={{ display:'flex', flexDirection:'column', gap:14 }}>

       {categories.map(function(cat) {

         return (

           <div key={cat.title} style={{ display:'flex', alignItems:'center', gap:16 }}>

             <div style={{ display:'flex', fontSize:10, fontWeight:700, color:cat.color, letterSpacing:'1px', width:80 }}>

               {cat.title.toUpperCase()}

             </div>

             <div style={{ display:'flex', flexWrap:'wrap', gap:7 }}>

               {cat.items.map(function(item) {

                 return (

                   <div key={item} style={{

                     display:'flex', padding:'4px 13px', borderRadius:6,

                     background:cat.color + '15', border:'1px solid ' + cat.color + '35',

                     color:'rgba(255,225,225,0.85)', fontSize:12, fontWeight:600,

                   }}>{item}</div>

                 );

               })}

             </div>

           </div>

         );

       })}

     </div>

   </div>

 );

})()


<br>

<p align="center"><sub>𝗉𝗈𝗐𝖾𝗋𝖾𝖽 𝖻𝗒 <a href="https://github.com/collectioneur/readme-aura">𝗋𝖾𝖺𝖽𝗆𝖾-𝖺𝗎𝗋𝖺</a></sub></p>