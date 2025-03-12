# hi
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>360 Business Magician Skills</title>
  <style>
    :root {
      --neon-pink: #ff00ff;
      --neon-pink-glow: #ff00ff80;
      --dark-bg: #0a0a12;
      --card-bg: rgba(20, 20, 35, 0.8);
    }
    
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'IBM Plex Mono', monospace;
    }
    
    body {
      background-color: var(--dark-bg);
      color: white;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      overflow-x: hidden;
      padding: 2rem;
      background: radial-gradient(circle at center, #1a1a2e 0%, #0a0a12 100%);
    }
    
    .container {
      max-width: 1200px;
      width: 100%;
      position: relative;
    }
    
    .header {
      text-align: center;
      margin-bottom: 3rem;
      position: relative;
    }
    
    .header h1 {
      font-size: 3rem;
      font-weight: 700;
      margin-bottom: 1rem;
      background: linear-gradient(90deg, #ff00ff, #ff66ff);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
      text-shadow: 0 0 15px var(--neon-pink-glow);
      letter-spacing: 2px;
    }
    
    .header p {
      font-size: 1.2rem;
      color: rgba(255, 255, 255, 0.8);
      max-width: 800px;
      margin: 0 auto;
      line-height: 1.6;
    }
    
    .skills-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
      gap: 2rem;
      margin-top: 2rem;
    }
    
    .skill-card {
      background: var(--card-bg);
      border-radius: 12px;
      padding: 1.5rem;
      position: relative;
      transition: all 0.3s ease;
      backdrop-filter: blur(10px);
      border: 1px solid rgba(255, 0, 255, 0.2);
      box-shadow: 0 0 25px rgba(255, 0, 255, 0.15);
      height: 100%;
      display: flex;
      flex-direction: column;
    }
    
    .skill-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 0 30px rgba(255, 0, 255, 0.3);
      border: 1px solid rgba(255, 0, 255, 0.5);
    }
    
    .skill-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: linear-gradient(45deg, transparent, rgba(255, 0, 255, 0.1), transparent);
      background-size: 200% 200%;
      animation: shimmer 3s infinite;
      border-radius: 12px;
      z-index: -1;
    }
    
    .skill-card h3 {
      font-size: 1.4rem;
      color: var(--neon-pink);
      margin-bottom: 1rem;
      text-shadow: 0 0 8px var(--neon-pink-glow);
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }
    
    .skill-card ul {
      list-style: none;
      padding-left: 0.5rem;
    }
    
    .skill-card li {
      margin-bottom: 0.5rem;
      display: flex;
      align-items: center;
      position: relative;
      padding-left: 1.5rem;
    }
    
    .skill-card li::before {
      content: '•';
      color: var(--neon-pink);
      font-size: 1.2rem;
      position: absolute;
      left: 0;
      top: 0;
    }
    
    .progress-container {
      width: 100%;
      height: 6px;
      background: rgba(255, 255, 255, 0.1);
      border-radius: 3px;
      margin-top: auto;
      overflow: hidden;
      position: relative;
    }
    
    .progress-bar {
      height: 100%;
      border-radius: 3px;
      background: linear-gradient(90deg, var(--neon-pink), #ff66ff);
      box-shadow: 0 0 10px var(--neon-pink);
      transition: width 1.5s cubic-bezier(0.25, 1, 0.5, 1);
      width: 0;
    }
    
    .skill-level {
      font-size: 0.8rem;
      color: rgba(255, 255, 255, 0.7);
      text-align: right;
      margin-top: 0.25rem;
    }
    
    @keyframes shimmer {
      0% { background-position: 0% 0%; }
      50% { background-position: 100% 100%; }
      100% { background-position: 0% 0%; }
    }
    
    .particles-container {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      z-index: -1;
      overflow: hidden;
    }
    
    .particle {
      position: absolute;
      border-radius: 50%;
      background: rgba(255, 0, 255, 0.5);
      box-shadow: 0 0 10px var(--neon-pink);
      animation: float 15s infinite linear;
    }
    
    @keyframes float {
      0% {
        transform: translateY(0) rotate(0deg);
        opacity: 0;
      }
      10% {
        opacity: 1;
      }
      90% {
        opacity: 1;
      }
      100% {
        transform: translateY(-1000px) rotate(720deg);
        opacity: 0;
      }
    }
    
    @media (max-width: 768px) {
      .header h1 {
        font-size: 2.5rem;
      }
      
      .skills-grid {
        grid-template-columns: 1fr;
      }
    }
  </style>
</head>
<body>
  <div class="particles-container" id="particles"></div>
  
  <div class="container">
    <div class="header">
      <h1>360 BUSINESS MAGICIAN</h1>
      <p>
        Leveraging cutting-edge technology and lived experience to transform accessibility 
        for the Deaf and hard of hearing communities through innovative AI-powered solutions.
      </p>
    </div>
    
    <div class="skills-grid">
      <div class="skill-card">
        <h3>AI & Technology</h3>
        <ul>
          <li>AI-Powered Platform Development</li>
          <li>Machine Learning Integration</li>
          <li>Natural Language Processing</li>
          <li>Computer Vision Applications</li>
          <li>API Integration & Development</li>
        </ul>
        <div class="progress-container">
          <div class="progress-bar" data-progress="95"></div>
        </div>
        <div class="skill-level">Expert</div>
      </div>
      
      <div class="skill-card">
        <h3>Web Development</h3>
        <ul>
          <li>Advanced React & Next.js</li>
          <li>Modern JavaScript (ES6+)</li>
          <li>Responsive Design & Animation</li>
          <li>Progressive Web Applications</li>
          <li>Accessibility-First Design</li>
        </ul>
        <div class="progress-container">
          <div class="progress-bar" data-progress="90"></div>
        </div>
        <div class="skill-level">Expert</div>
      </div>
      
      <div class="skill-card">
        <h3>App Development</h3>
        <ul>
          <li>React Native Multi-Platform</li>
          <li>Swift & SwiftUI</li>
          <li>Kotlin & Android Development</li>
          <li>App Store Optimization</li>
          <li>Real-time Communication Tools</li>
        </ul>
        <div class="progress-container">
          <div class="progress-bar" data-progress="85"></div>
        </div>
        <div class="skill-level">Advanced</div>
      </div>
      
      <div class="skill-card">
        <h3>Google Ecosystem</h3>
        <ul>
          <li>Google Cloud Platform</li>
          <li>Firebase Integration</li>
          <li>Google Workspace Solutions</li>
          <li>DialogFlow & Assistant</li>
          <li>Analytics & Performance Tools</li>
        </ul>
        <div class="progress-container">
          <div class="progress-bar" data-progress="88"></div>
        </div>
        <div class="skill-level">Advanced</div>
      </div>
      
      <div class="skill-card">
        <h3>Entrepreneurship</h3>
        <ul>
          <li>Startup Development</li>
          <li>Business Model Innovation</li>
          <li>Strategic Partnership Building</li>
          <li>Financial Planning Services</li>
          <li>Venture Capital Acquisition</li>
        </ul>
        <div class="progress-container">
          <div class="progress-bar" data-progress="92"></div>
        </div>
        <div class="skill-level">Expert</div>
      </div>
      
      <div class="skill-card">
        <h3>Accessibility Expertise</h3>
        <ul>
          <li>Sign Language Translation</li>
          <li>Document Simplification</li>
          <li>WCAG & ADA Compliance</li>
          <li>Deaf-Specific UX/UI Design</li>
          <li>Inclusive Communication Systems</li>
        </ul>
        <div class="progress-container">
          <div class="progress-bar" data-progress="98"></div>
        </div>
        <div class="skill-level">Expert</div>
      </div>
    </div>
  </div>
  
  <script>
    // Animate progress bars on load
    document.addEventListener('DOMContentLoaded', () => {
      setTimeout(() => {
        const progressBars = document.querySelectorAll('.progress-bar');
        progressBars.forEach(bar => {
          const progress = bar.getAttribute('data-progress');
          bar.style.width = `${progress}%`;
        });
      }, 300);
      
      // Create floating particles
      const particlesContainer = document.getElementById('particles');
      const particleCount = 30;
      
      for (let i = 0; i < particleCount; i++) {
        createParticle();
      }
      
      function createParticle() {
        const particle = document.createElement('div');
        particle.classList.add('particle');
        
        // Random size between 2px and 8px
        const size = Math.random() * 6 + 2;
        particle.style.width = `${size}px`;
        particle.style.height = `${size}px`;
        
        // Random position
        const posX = Math.random() * 100;
        const posY = Math.random() * 100 + 100;
        particle.style.left = `${posX}%`;
        particle.style.bottom = `${-posY}px`;
        
        // Random delay and duration
        const delay = Math.random() * 10;
        const duration = Math.random() * 10 + 10;
        particle.style.animationDelay = `${delay}s`;
        particle.style.animationDuration = `${duration}s`;
        
        particlesContainer.appendChild(particle);
        
        // Remove and recreate particle after animation completes
        setTimeout(() => {
          particle.remove();
          createParticle();
        }, (delay + duration) * 1000);
      }
    });
  </script>
</body>
</html>
