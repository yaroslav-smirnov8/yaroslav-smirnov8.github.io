---
layout: default
title: Matrix Teaching Quest - Interactive Quest System
---

<div class="project-hero">
  <div class="container">
    <h1>Matrix Teaching Quest</h1>
    <p class="project-subtitle">Interactive quest + promo funnel with first-party analytics</p>
    <div class="project-tech-stack">
      <span class="tech-tag">FastAPI</span>
      <span class="tech-tag">React</span>
      <span class="tech-tag">PostgreSQL</span>
      <span class="tech-tag">Async</span>
      <span class="tech-tag">Analytics</span>
    </div>
  </div>
</div>

<div class="project-overview">
  <div class="container">
    <div class="overview-content">
      <div class="overview-text">
        <h2>Project Overview</h2>
        <p>Built a Matrix-themed, branching learning experience that converts user engagement into measured activation. Async FastAPI services drive quest logic, achievements, and unique promo codes; React delivers cinematic UX with local resilience. A first-party analytics pipeline captures device/fingerprint/session data, feeding a secured admin layer with funnels and exports.</p>
      </div>
      <div class="overview-features">
        <h3>Key Features</h3>
        <ul>
          <li>Branching quest scenes with hidden choices and easter eggs</li>
          <li>Achievement system with progress tracking</li>
          <li>Unique single-use promo codes tied to course URLs</li>
          <li>First-party analytics without third-party dependencies</li>
          <li>Admin dashboard with KPIs, funnels, and CSV/JSON export</li>
          <li>Telegram WebApp integration plus web fallback</li>
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
        <p>The system implements a clean, async-first architecture with clear separation of concerns:</p>
        <ul>
          <li><strong>Backend</strong>: FastAPI (async) with modular routers for quest, user, achievements, promo, admin, and analytics</li>
          <li><strong>Data Layer</strong>: PostgreSQL via async SQLAlchemy with Alembic migrations</li>
          <li><strong>Services</strong>: QuestService (scenes and branching), AchievementService (promo bonuses), PromoService (unique codes)</li>
          <li><strong>Analytics</strong>: First-party pipeline capturing device/fingerprint/session data</li>
          <li><strong>Frontend</strong>: React with styled-components and framer-motion for cinematic UX</li>
        </ul>
      </div>
      <div class="architecture-diagram">
        <img src="/assets/images/matrix-quest-architecture.png" alt="Matrix Teaching Quest Architecture" class="architecture-image">
        <p class="image-caption">Async FastAPI backend with React frontend and first-party analytics</p>
      </div>
    </div>
  </div>
</div>

<div class="project-features">
  <div class="container">
    <h2>Key Features & Implementation</h2>
    <div class="features-grid">
      <div class="feature-item">
        <h3>Interactive Quest System</h3>
        <ul>
          <li>Branching narrative with multiple paths and outcomes</li>
          <li>Hidden choices and easter eggs for engagement</li>
          <li>Cinematic transitions and effects using framer-motion</li>
          <li>Local progress persistence for resilience</li>
          <li>Telegram WebApp integration with web fallback</li>
        </ul>
      </div>
      <div class="feature-item">
        <h3>Achievement & Promo System</h3>
        <ul>
          <li>Achievement tracking with requirements and rewards</li>
          <li>Unique single-use promo code generation</li>
          <li>Promo code validation and usage tracking</li>
          <li>Integration with external course platform</li>
          <li>Admin management of achievements and rewards</li>
        </ul>
      </div>
      <div class="feature-item">
        <h3>First-Party Analytics</h3>
        <ul>
          <li>Event tracking without external dependencies</li>
          <li>Device fingerprinting and session management</li>
          <li>Funnel analysis and conversion tracking</li>
          <li>Admin dashboard with real-time metrics</li>
          <li>CSV/JSON export for further analysis</li>
        </ul>
      </div>
      <div class="feature-item">
        <h3>Admin Dashboard</h3>
        <ul>
          <li>HTTP Basic Authentication for security</li>
          <li>Overview analytics with key metrics</li>
          <li>Scene funnel analysis</li>
          <li>Promo usage tracking</li>
          <li>User management and data export</li>
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
          <li>FastAPI (async) with modular routers</li>
          <li>SQLAlchemy async with asyncpg driver</li>
          <li>Pydantic for data validation</li>
          <li>Alembic for database migrations</li>
        </ul>
      </div>
      <div class="tech-category">
        <h3>Frontend</h3>
        <ul>
          <li>React 18 with modern hooks</li>
          <li>styled-components for styling</li>
          <li>framer-motion for animations</li>
          <li>Telegram WebApp integration</li>
        </ul>
      </div>
      <div class="tech-category">
        <h3>Database</h3>
        <ul>
          <li>PostgreSQL as primary database</li>
          <li>JSON columns for flexible data structures</li>
          <li>Indexes for performance optimization</li>
          <li>Relationship management for data integrity</li>
        </ul>
      </div>
      <div class="tech-category">
        <h3>Security & Deployment</h3>
        <ul>
          <li>HTTP Basic Auth for admin endpoints</li>
          <li>CORS configuration for allowed origins</li>
          <li>Environment-based configuration</li>
          <li>Docker support for deployment</li>
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
        <h3>Async Orchestration</h3>
        <p>Implemented async FastAPI services to handle quest state and promo generation. Ensured proper session management and error handling throughout the application.</p>
      </div>
      <div class="challenge-item">
        <h3>Promo Uniqueness</h3>
        <p>Designed system to generate unique, single-use promo codes with proper validation. Implemented database constraints and application-level checks to prevent duplication.</p>
      </div>
      <div class="challenge-item">
        <h3>First-Party Analytics</h3>
        <p>Built custom analytics pipeline without third-party dependencies. Implemented device fingerprinting, session management, and event tracking for comprehensive user behavior analysis.</p>
      </div>
      <div class="challenge-item">
        <h3>Admin Security</h3>
        <p>Secured admin endpoints with HTTP Basic Authentication and constrained CORS. Implemented proper authorization checks and data access controls.</p>
      </div>
    </div>
  </div>
</div>

<div class="project-impact">
  <div class="container">
    <h2>Technical Achievements</h2>
    <div class="impact-content">
      <div class="impact-highlights">
        <h3>Key Technical Highlights</h3>
        <ul>
          <li><strong>Async-First Design</strong>: FastAPI with async SQLAlchemy for high concurrency</li>
          <li><strong>First-Party Analytics</strong>: Custom analytics pipeline without external dependencies</li>
          <li><strong>Branching Logic</strong>: Complex quest system with multiple paths and outcomes</li>
          <li><strong>Promo System</strong>: Unique, single-use promo codes with validation</li>
          <li><strong>Admin Dashboard</strong>: Secure interface for analytics and management</li>
        </ul>
      </div>
      <div class="impact-value">
        <h3>Business Value</h3>
        <ul>
          <li>Engaging user experience with gamification elements</li>
          <li>Conversion funnel with measurable activation metrics</li>
          <li>Data ownership with first-party analytics</li>
          <li>Scalable architecture for growth</li>
          <li>Secure admin operations with proper authentication</li>
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
          <img src="/assets/images/matrix-quest-demo.png" alt="Matrix Teaching Quest Demo">
          <div class="play-button">
            <a href="#" target="_blank">Watch Demo</a>
          </div>
        </div>
      </div>
      <div class="demo-highlights">
        <h3>Key Features in Action</h3>
        <ul>
          <li>Interactive quest with branching choices</li>
          <li>Achievement unlocking and progress tracking</li>
          <li>Promo code generation and validation</li>
          <li>Admin dashboard with analytics</li>
          <li>Funnel analysis and export capabilities</li>
        </ul>
      </div>
    </div>
  </div>
</div>

<div class="project-navigation">
  <div class="container">
    <div class="nav-links">
      <a href="/projects/invbot/" class="nav-link">← Previous Project</a>
      <a href="/projects/platform-teachers/" class="nav-link">Next Project →</a>
    </div>
  </div>
</div>