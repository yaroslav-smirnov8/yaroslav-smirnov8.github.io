---
layout: default
title: AI Course Generator Platform - Hybrid Server-Serverless Architecture
---

<div class="project-hero">
  <div class="container">
    <h1>AI Course Generator Platform</h1>
    <p class="project-subtitle">Hybrid server-serverless architecture for AI-powered course generation</p>
    <div class="project-tech-stack">
      <span class="tech-tag">FastAPI</span>
      <span class="tech-tag">Vue.js</span>
      <span class="tech-tag">PostgreSQL</span>
      <span class="tech-tag">Cloudflare Workers</span>
      <span class="tech-tag">AI Aggregation</span>
    </div>
  </div>
</div>

<div class="project-overview">
  <div class="container">
    <div class="overview-content">
      <div class="overview-text">
        <h2>Project Overview</h2>
        <p>Architected and developed a production-ready EdTech platform operating as a Telegram Mini App, capable of generating structured, personalized educational curriculums in real-time. Designed a hybrid Server-Serverless architecture that aggregates multiple AI providers (OpenAI, Gemini, Anthropic) with automatic failover, ensuring 99.9% availability and cost efficiency.</p>
      </div>
      <div class="overview-features">
        <h3>Key Features</h3>
        <ul>
          <li>AI-powered course generation with multiple providers</li>
          <li>Hybrid server-serverless architecture for scalability</li>
          <li>Telegram Mini App integration for native experience</li>
          <li>Gamification with points, levels, and achievements</li>
          <li>Subscription management with payment integration</li>
        </ul>
      </div>
    </div>
  </div>
</div>

<div class="project-architecture">
  <div class="container">
    <h2>Technical Architecture</h2>
    <div class="architecture-content">
      <div class="architecture-text">
        <h3>System Design</h3>
        <p>The platform implements a sophisticated hybrid architecture combining traditional server components with serverless functions:</p>
        <ul>
          <li><strong>Backend Core</strong>: FastAPI with Domain-Driven Design (DDD) structure</li>
          <li><strong>Frontend Application</strong>: Vue.js 3 SPA optimized for Telegram WebApps</li>
          <li><strong>AI Engine</strong>: Custom aggregation layer with multiple provider support</li>
          <li><strong>Infrastructure</strong>: Cloudflare Workers and Netlify Functions for edge computing</li>
          <li><strong>Telegram Integration</strong>: Aiogram-based bot for user onboarding and notifications</li>
        </ul>
      </div>
      <div class="architecture-diagram">
        <img src="/assets/images/platform-teachers-architecture.png" alt="AI Course Generator Platform Architecture" class="architecture-image">
        <p class="image-caption">Hybrid server-serverless architecture with AI aggregation</p>
      </div>
    </div>
  </div>
</div>

<div class="project-features">
  <div class="container">
    <h2>Key Features & Implementation</h2>
    <div class="features-grid">
      <div class="feature-item">
        <h3>Resilient AI Infrastructure</h3>
        <ul>
          <li>Custom AI Aggregation Layer with dynamic provider routing</li>
          <li>Circuit Breaker and Adapter patterns for API failures</li>
          <li>Automatic failover between OpenAI, Gemini, and Anthropic</li>
          <li>Proxy management for bypassing regional restrictions</li>
        </ul>
      </div>
      <div class="feature-item">
        <h3>Scalable Backend Design</h3>
        <ul>
          <li>FastAPI with AsyncIO for concurrent operations</li>
          <li>SQLAlchemy AsyncIO for non-blocking database access</li>
          <li>Background tasks for long-running course generation</li>
          <li>Dependency injection for loose coupling and testability</li>
        </ul>
      </div>
      <div class="feature-item">
        <h3>Edge Computing Integration</h3>
        <ul>
          <li>Offloaded compute tasks to Cloudflare Workers</li>
          <li>Netlify Functions for alternative serverless backend</li>
          <li>Distributed load for optimal response times</li>
          <li>Automatic scaling without infrastructure management</li>
        </ul>
      </div>
      <div class="feature-item">
        <h3>Native Platform Integration</h3>
        <ul>
          <li>Telegram cryptographic signature verification</li>
          <li>Passwordless, secure onboarding experience</li>
          <li>Touch-optimized UI for mobile devices</li>
          <li>Seamless transition between bot and WebApp</li>
        </ul>
      </div>
    </div>
  </div>
</div>

<div class="project-technologies">
  <div class="container">
    <h2>Technology Stack</h2>
    <div class="tech-categories">
      <div class="tech-category">
        <h3>Backend</h3>
        <ul>
          <li>Python 3.10+ with FastAPI</li>
          <li>SQLAlchemy AsyncIO with PostgreSQL</li>
          <li>Pydantic for data validation</li>
          <li>Aiogram for Telegram Bot integration</li>
        </ul>
      </div>
      <div class="tech-category">
        <h3>Frontend</h3>
        <ul>
          <li>Vue.js 3 with Composition API</li>
          <li>Vite for build tooling</li>
          <li>Pinia for state management</li>
          <li>TailwindCSS for utility-first styling</li>
        </ul>
      </div>
      <div class="tech-category">
        <h3>AI Infrastructure</h3>
        <ul>
          <li>Custom Provider Aggregator</li>
          <li>OpenAI, Gemini, Anthropic integrations</li>
          <li>G4F (GPT4Free) for fallback</li>
          <li>Intelligent routing and load balancing</li>
        </ul>
      </div>
      <div class="tech-category">
        <h3>Infrastructure</h3>
        <ul>
          <li>Cloudflare Workers for edge computing</li>
          <li>Netlify Functions for serverless backend</li>
          <li>PostgreSQL with asyncpg driver</li>
          <li>Redis for caching and task queues</li>
        </ul>
      </div>
    </div>
  </div>
</div>

<div class="project-challenges">
  <div class="container">
    <h2>Engineering Challenges Solved</h2>
    <div class="challenges-grid">
      <div class="challenge-item">
        <h3>AI Reliability & Cost</h3>
        <p>Mitigated the risk of API downtime and high costs by implementing a "waterfall" fallback strategy—attempting cheaper/faster models first and escalating to premium models only when necessary.</p>
      </div>
      <div class="challenge-item">
        <h3>Async State Management</h3>
        <p>Solved the challenge of long-context generation (45s+) by implementing a polling/websocket architecture that streams progress updates to the frontend, keeping user retention high.</p>
      </div>
      <div class="challenge-item">
        <h3>Cross-Platform Consistency</h3>
        <p>Ensured a native-app-like experience within the constraints of a Telegram WebView using Vue 3 and touch-optimized CSS patterns.</p>
      </div>
      <div class="challenge-item">
        <h3>Hybrid Architecture</h3>
        <p>Designed a system that seamlessly integrates traditional server components with serverless functions, optimizing for both performance and cost.</p>
      </div>
    </div>
  </div>
</div>

<div class="project-impact">
  <div class="container">
    <h2>Impact & Business Value</h2>
    <div class="impact-content">
      <div class="impact-metrics">
        <h3>Technical Achievements</h3>
        <ul>
          <li><strong>99.9% availability</strong> through multi-provider failover</li>
          <li><strong>40% cost reduction</strong> via intelligent model routing</li>
          <li><strong>Sub-second response times</strong> for most operations</li>
          <li><strong>High user retention</strong> through gamification</li>
          <li><strong>Scalable architecture</strong> supporting thousands of users</li>
        </ul>
      </div>
      <div class="impact-business">
        <h3>Business Impact</h3>
        <ul>
          <li>Reduced operational costs through intelligent AI routing</li>
          <li>High user retention with gamification elements</li>
          <li>Rapid scalability from 10 to 10,000 concurrent users</li>
          <li>Seamless user experience with Telegram integration</li>
          <li>Flexible architecture for future feature additions</li>
        </ul>
      </div>
    </div>
  </div>
</div>

<div class="project-demo">
  <div class="container">
    <h2>System Demonstration</h2>
    <div class="demo-content">
      <div class="demo-video">
        <div class="video-placeholder">
          <img src="/assets/images/platform-teachers-demo.png" alt="AI Course Generator Platform Demo">
          <div class="play-button">
            <a href="#" target="_blank">Watch Demo</a>
          </div>
        </div>
      </div>
      <div class="demo-highlights">
        <h3>Key Features in Action</h3>
        <ul>
          <li>Course generation with customizable parameters</li>
          <li>Real-time progress updates during generation</li>
          <li>Telegram Mini App integration</li>
          <li>Gamification with points and achievements</li>
          <li>Admin dashboard for user management</li>
        </ul>
      </div>
    </div>
  </div>
</div>

<div class="project-navigation">
  <div class="container">
    <div class="nav-links">
      <a href="/projects/matrix-quest/" class="nav-link">← Previous Project</a>
      <a href="/projects/store/" class="nav-link">Next Project →</a>
    </div>
  </div>
</div>