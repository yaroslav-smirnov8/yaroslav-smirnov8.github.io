---
layout: null
---

/* Portfolio CSS Styles */

/* Global Styles */
:root {
  --primary-color: #2563eb;
  --secondary-color: #64748b;
  --accent-color: #3b82f6;
  --background-color: #ffffff;
  --text-color: #1f2937;
  --light-gray: #f3f4f6;
  --border-color: #e5e7eb;
  --shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
  --shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  line-height: 1.6;
  color: var(--text-color);
  background-color: var(--background-color);
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

/* Typography */
h1, h2, h3 {
  font-weight: 600;
  line-height: 1.25;
  margin-bottom: 1rem;
}

h1 {
  font-size: 2.5rem;
  color: var(--primary-color);
}

h2 {
  font-size: 2rem;
  color: var(--text-color);
  border-bottom: 2px solid var(--border-color);
  padding-bottom: 0.5rem;
  margin-bottom: 2rem;
}

h3 {
  font-size: 1.5rem;
  color: var(--text-color);
}

p {
  margin-bottom: 1rem;
  font-size: 1.1rem;
}

a {
  color: var(--primary-color);
  text-decoration: none;
  transition: color 0.2s ease;
}

a:hover {
  color: var(--accent-color);
}

/* Hero Section */
.hero-section {
  background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
  color: white;
  padding: 5rem 0;
  text-align: center;
}

.hero-content h1 {
  color: white;
  font-size: 3rem;
  margin-bottom: 0.5rem;
}

.hero-subtitle {
  font-size: 1.25rem;
  margin-bottom: 2rem;
  opacity: 0.9;
}

.hero-cta {
  margin-top: 2rem;
}

.btn {
  display: inline-block;
  padding: 0.75rem 1.5rem;
  margin: 0 0.5rem;
  border-radius: 0.375rem;
  font-weight: 500;
  text-align: center;
  text-decoration: none;
  transition: all 0.2s ease;
  cursor: pointer;
  border: 1px solid transparent;
}

.btn-primary {
  background-color: white;
  color: var(--primary-color);
}

.btn-primary:hover {
  background-color: var(--light-gray);
}

.btn-secondary {
  background-color: transparent;
  color: white;
  border: 1px solid white;
}

.btn-secondary:hover {
  background-color: rgba(255, 255, 255, 0.1);
}

/* Section Styles */
.section-title {
  text-align: center;
  margin-bottom: 3rem;
  position: relative;
}

.section-title::after {
  content: '';
  position: absolute;
  bottom: -10px;
  left: 50%;
  transform: translateX(-50%);
  width: 60px;
  height: 4px;
  background-color: var(--primary-color);
  border-radius: 2px;
}

/* Highlights Section */
.highlights-section {
  padding: 4rem 0;
  background-color: var(--light-gray);
}

.highlights-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
}

.highlight-card {
  background-color: white;
  padding: 2rem;
  border-radius: 0.5rem;
  box-shadow: var(--shadow);
  text-align: center;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.highlight-card:hover {
  transform: translateY(-5px);
  box-shadow: var(--shadow-lg);
}

.highlight-card h3 {
  color: var(--primary-color);
  margin-bottom: 1rem;
}

/* Projects Section */
.projects-section {
  padding: 4rem 0;
}

.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 2rem;
}

.project-card {
  background-color: white;
  border-radius: 0.5rem;
  overflow: hidden;
  box-shadow: var(--shadow);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  display: flex;
  flex-direction: column;
}

.project-card:hover {
  transform: translateY(-5px);
  box-shadow: var(--shadow-lg);
}

.project-image {
  height: 200px;
  overflow: hidden;
}

.project-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.3s ease;
}

.project-card:hover .project-image img {
  transform: scale(1.05);
}

.project-content {
  padding: 1.5rem;
  flex-grow: 1;
  display: flex;
  flex-direction: column;
}

.project-content h3 {
  margin-bottom: 0.5rem;
}

.project-tech {
  font-size: 0.9rem;
  color: var(--secondary-color);
  margin-bottom: 1rem;
}

.project-desc {
  margin-bottom: 1.5rem;
  flex-grow: 1;
}

.project-link {
  align-self: flex-start;
  background-color: var(--primary-color);
  color: white;
  padding: 0.5rem 1rem;
  border-radius: 0.25rem;
  font-size: 0.9rem;
  transition: background-color 0.2s ease;
}

.project-link:hover {
  background-color: var(--accent-color);
}

/* Tech Tags */
.tech-tag {
  display: inline-block;
  background-color: var(--light-gray);
  color: var(--text-color);
  padding: 0.25rem 0.5rem;
  margin: 0.25rem;
  border-radius: 0.25rem;
  font-size: 0.8rem;
  font-weight: 500;
}

/* Skills Section */
.skills-preview-section {
  padding: 4rem 0;
  background-color: var(--light-gray);
}

.skills-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
}

.skill-category h3 {
  color: var(--primary-color);
  margin-bottom: 1rem;
}

.skill-category ul {
  list-style-type: none;
  padding-left: 0;
}

.skill-category li {
  padding: 0.5rem 0;
  border-bottom: 1px solid var(--border-color);
}

/* Contact Section */
.contact-section {
  padding: 4rem 0;
  text-align: center;
}

.contact-methods {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 2rem;
  margin: 2rem 0;
}

.contact-item {
  padding: 1.5rem;
  background-color: var(--light-gray);
  border-radius: 0.5rem;
}

.contact-item h3 {
  color: var(--primary-color);
  margin-bottom: 0.5rem;
}

/* Project Navigation */
.project-navigation {
  padding: 2rem 0;
  background-color: var(--light-gray);
}

.nav-links {
  display: flex;
  justify-content: space-between;
  max-width: 800px;
  margin: 0 auto;
}

.nav-link {
  display: inline-block;
  padding: 0.75rem 1.5rem;
  background-color: white;
  color: var(--primary-color);
  border-radius: 0.375rem;
  font-weight: 500;
  text-decoration: none;
  transition: all 0.2s ease;
  box-shadow: var(--shadow);
}

.nav-link:hover {
  background-color: var(--primary-color);
  color: white;
}

/* Responsive Design */
@media (max-width: 768px) {
  .container {
    padding: 0 15px;
  }
  
  h1 {
    font-size: 2rem;
  }
  
  .hero-content h1 {
    font-size: 2.5rem;
  }
  
  .projects-grid {
    grid-template-columns: 1fr;
  }
  
  .highlights-grid {
    grid-template-columns: 1fr;
  }
  
  .skills-grid {
    grid-template-columns: 1fr;
  }
  
  .contact-methods {
    grid-template-columns: 1fr;
  }
  
  .nav-links {
    flex-direction: column;
    align-items: center;
    gap: 1rem;
  }
}