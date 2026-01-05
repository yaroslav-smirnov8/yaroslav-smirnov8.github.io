---
layout: default
title: Train Prompts Bot - Prompt Engineering Tutor
---

<div class="project-hero">
  <div class="container">
    <h1>Train Prompts Bot</h1>
    <p class="project-subtitle">Educational bot teaching prompt engineering with AI feedback</p>
    <div class="project-tech-stack">
      <span class="tech-tag">Python</span>
      <span class="tech-tag">aiogram 3</span>
      <span class="tech-tag">PostgreSQL</span>
      <span class="tech-tag">AI Integration</span>
      <span class="tech-tag">Quizzes</span>
    </div>
  </div>
</div>

<div class="project-overview">
  <div class="container">
    <div class="overview-content">
      <div class="overview-text">
        <h2>Project Overview</h2>
        <p>Built an async Telegram bot that teaches prompt engineering for text and images through guided lessons, quizzes, and hands-on AI generation. The system features structured lessons with step-by-step navigation, AI-powered content generation with daily quotas, quizzes auto-graded by an LLM, user ratings leaderboard, and an admin console for user management and statistics.</p>
      </div>
      <div class="overview-features">
        <h3>Key Features</h3>
        <ul>
          <li>Guided text & image prompt lessons with step navigation</li>
          <li>AI-powered text/image generation with daily quotas</li>
          <li>Quizzes auto-graded by an LLM with user ratings</li>
          <li>Admin console for user management and stats</li>
          <li>Rich inline keyboards for smooth UX</li>
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
        <p>The bot implements a clean, modular architecture with clear separation of concerns:</p>
        <ul>
          <li><strong>Bot Core</strong>: aiogram 3 dispatcher with middlewares and routers</li>
          <li><strong>Handlers</strong>: Organized by domain (basic, admin, lessons, generation, quizzes)</li>
          <li><strong>Services</strong>: AI generation, lesson management, quiz evaluation</li>
          <li><strong>Data Layer</strong>: Async SQLAlchemy models with CRUD helpers</li>
          <li><strong>Middlewares</strong>: DB session, access control, error handling</li>
        </ul>
      </div>
      <div class="architecture-diagram">
        <img src="/assets/images/train-prompts-bot-architecture.png" alt="Train Prompts Bot Architecture" class="architecture-image">
        <p class="image-caption">Async architecture with modular routers and services</p>
      </div>
    </div>
  </div>
</div>

<div class="project-features">
  <div class="container">
    <h2>Key Features & Implementation</h2>
    <div class="features-grid">
      <div class="feature-item">
        <h3>Educational Content</h3>
        <ul>
          <li>Structured lessons with ordered steps</li>
          <li>Prompt examples for best practices</li>
          <li>Progress tracking per user</li>
          <li>Completion statistics and ratings</li>
        </ul>
      </div>
      <div class="feature-item">
        <h3>AI Integration</h3>
        <ul>
          <li>Text generation via LLM7 API</li>
          <li>Image generation via Together AI</li>
          <li>Daily quota management for non-admin users</li>
          <li>AI-powered quiz answer evaluation</li>
        </ul>
      </div>
      <div class="feature-item">
        <h3>Database Design</h3>
        <ul>
          <li>PostgreSQL with asyncpg driver</li>
          <li>Models for users, lessons, progress, quizzes</li>
          <li>Relationship management between entities</li>
          <li>Aggregation queries for ratings and statistics</li>
        </ul>
      </div>
      <div class="feature-item">
        <h3>Admin & Management</h3>
          <ul>
          <li>Admin-only commands and filters</li>
          <li>User statistics and management</li>
          <li>Admin role assignment from environment</li>
          <li>System health monitoring</li>
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
        <h3>Backend & Framework</h3>
        <ul>
          <li>Python 3 with asyncio</li>
          <li>aiogram 3 for Telegram Bot API</li>
          <li>SQLAlchemy async ORM</li>
          <li>asyncpg PostgreSQL driver</li>
        </ul>
      </div>
      <div class="tech-category">
        <h3>AI & Integration</h3>
        <ul>
          <li>LLM7 API for text generation</li>
          <li>Together AI for image generation</li>
          <li>aiohttp for async HTTP requests</li>
          <li>Dynamic provider loading with retries</li>
        </ul>
      </div>
      <div class="tech-category">
        <h3>Database & Storage</h3>
        <ul>
          <li>PostgreSQL as primary database</li>
          <li>File system for generated images</li>
          <li>Migration scripts for schema evolution</li>
          <li>CRUD helpers for data operations</li>
        </ul>
      </div>
      <div class="tech-category">
        <h3>DevOps & Configuration</h3>
        <ul>
          <li>Environment-based configuration</li>
          <li>Structured logging with loguru</li>
          <li>Startup content seeding</li>
          <li>Defensive error handling</li>
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
        <h3>Unstable AI Providers</h3>
        <p>Added retry-capable provider selection, timeouts, and graceful fallbacks to ensure reliable AI generation even when individual providers experience issues.</p>
      </div>
      <div class="challenge-item">
        <h3>Per-Update DB Safety</h3>
        <p>Implemented session middleware with commit/rollback safety to prevent partial writes and ensure data consistency during concurrent operations.</p>
      </div>
      <div class="challenge-item">
        <h3>User Abuse Prevention</h3>
        <p>Implemented daily generation quotas with automatic reset and admin bypass to prevent abuse while ensuring fair usage.</p>
      </div>
      <div class="challenge-item">
        <h3>Content Consistency</h3>
        <p>Created startup seeding pipeline for lessons and quizzes to keep environments aligned and ensure consistent content across deployments.</p>
      </div>
    </div>
  </div>
</div>

<div class="project-impact">
  <div class="container">
    <h2>Impact & Educational Value</h2>
    <div class="impact-content">
      <div class="impact-metrics">
        <h3>Technical Achievements</h3>
        <ul>
          <li><strong>End-to-end async architecture</strong> for high concurrency</li>
          <li><strong>Modular design</strong> with clear separation of concerns</li>
          <li><strong>Robust error handling</strong> with graceful degradation</li>
          <li><strong>Secure admin controls</strong> with role-based access</li>
          <li><strong>Scalable data model</strong> for content growth</li>
        </ul>
      </div>
      <div class="impact-business">
        <h3>Educational Value</h3>
        <ul>
          <li>Structured learning path for prompt engineering</li>
          <li>Immediate AI feedback for skill development</li>
          <li>Progress tracking and motivation through ratings</li>
          <li>Hands-on practice with real AI systems</li>
          <li>Scalable platform for content expansion</li>
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
          <img src="/assets/images/train-prompts-bot-demo.png" alt="Train Prompts Bot Demo">
          <div class="play-button">
            <a href="#" target="_blank">Watch Demo</a>
          </div>
        </div>
      </div>
      <div class="demo-highlights">
        <h3>Key Features in Action</h3>
        <ul>
          <li>Lesson navigation with step-by-step progress</li>
          <li>AI-powered text and image generation</li>
          <li>Quiz system with AI evaluation</li>
          <li>User ratings and leaderboard</li>
          <li>Admin console for management</li>
        </ul>
      </div>
    </div>
  </div>
</div>

<div class="project-navigation">
  <div class="container">
    <div class="nav-links">
      <a href="/projects/teacherhelper/" class="nav-link">← Previous Project</a>
      <a href="/projects/" class="nav-link">Back to Projects</a>
    </div>
  </div>
</div>