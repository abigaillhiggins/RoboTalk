---
layout: default
title: About
permalink: /about/
---

<div class="about-container">
    <header class="about-header">
        <h1 class="about-title">About {{ site.title }}</h1>
        <div class="about-subtitle">Exploring the Future of Technology</div>
    </header>

    <section class="about-content">
        <div class="about-section">
            <h2>Our Mission</h2>
            <p>At {{ site.title }}, we're passionate about exploring and sharing the latest developments in robotics, artificial intelligence, and cutting-edge technology. Our mission is to make complex technological concepts accessible while fostering meaningful discussions about their impact on society.</p>
        </div>

        <div class="about-section">
            <h2>Who We Are</h2>
            <p>We're a team of technology enthusiasts, researchers, and industry professionals dedicated to bringing you insightful analysis and commentary on the rapidly evolving world of robotics and AI. Our diverse backgrounds allow us to approach topics from multiple perspectives, ensuring comprehensive coverage of the tech landscape.</p>
        </div>

        <div class="about-section">
            <h2>What We Cover</h2>
            <div class="topics-grid">
                <div class="topic-card">
                    <h3>Robotics</h3>
                    <ul>
                        <li>Autonomous Systems</li>
                        <li>Industrial Automation</li>
                        <li>Human-Robot Interaction</li>
                        <li>Soft Robotics</li>
                    </ul>
                </div>
                <div class="topic-card">
                    <h3>Artificial Intelligence</h3>
                    <ul>
                        <li>Machine Learning</li>
                        <li>Neural Networks</li>
                        <li>Computer Vision</li>
                        <li>Natural Language Processing</li>
                    </ul>
                </div>
                <div class="topic-card">
                    <h3>Future Tech</h3>
                    <ul>
                        <li>Quantum Computing</li>
                        <li>Brain-Computer Interfaces</li>
                        <li>Internet of Things</li>
                        <li>Emerging Technologies</li>
                    </ul>
                </div>
            </div>
        </div>

        <div class="about-section">
            <h2>Get Involved</h2>
            <p>We believe in the power of community and welcome contributions from our readers. Whether you're a seasoned professional or just starting your journey in technology, there are many ways to get involved:</p>
            <ul class="involvement-list">
                <li>Share your insights through comments</li>
                <li>Suggest topics for future articles</li>
                <li>Contribute guest posts</li>
                <li>Join our Discord community</li>
            </ul>
        </div>

        <div class="about-section">
            <h2>Contact Us</h2>
            <p>Have questions or suggestions? We'd love to hear from you! Reach out to us at <a href="mailto:{{ site.email }}">{{ site.email }}</a> or connect with us on social media:</p>
            <div class="social-links">
                {% if site.github_username %}
                <a href="https://github.com/{{ site.github_username }}" class="social-link" target="_blank">GitHub</a>
                {% endif %}
                {% if site.twitter_username %}
                <a href="https://twitter.com/{{ site.twitter_username }}" class="social-link" target="_blank">Twitter</a>
                {% endif %}
                {% if site.linkedin_username %}
                <a href="https://linkedin.com/in/{{ site.linkedin_username }}" class="social-link" target="_blank">LinkedIn</a>
                {% endif %}
            </div>
        </div>
    </section>
</div>

<style>
.about-container {
    max-width: 900px;
    margin: 0 auto;
    padding: 2rem 0;
}

.about-header {
    text-align: center;
    margin-bottom: 4rem;
}

.about-title {
    font-size: 3rem;
    margin-bottom: 1rem;
    background: linear-gradient(120deg, var(--primary-color), var(--accent-color));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

.about-subtitle {
    font-size: 1.2rem;
    color: rgba(255, 255, 255, 0.8);
}

.about-section {
    margin-bottom: 4rem;
}

.about-section h2 {
    font-size: 2rem;
    margin-bottom: 1.5rem;
    color: var(--primary-color);
}

.about-section p {
    font-size: 1.1rem;
    line-height: 1.8;
    color: rgba(255, 255, 255, 0.9);
    margin-bottom: 1.5rem;
}

.topics-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
    margin-top: 2rem;
}

.topic-card {
    background: rgba(255, 255, 255, 0.05);
    border: 1px solid rgba(0, 255, 157, 0.2);
    border-radius: 8px;
    padding: 1.5rem;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.topic-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(0, 255, 157, 0.1);
}

.topic-card h3 {
    color: var(--accent-color);
    margin-bottom: 1rem;
}

.topic-card ul {
    list-style: none;
    padding: 0;
}

.topic-card li {
    margin-bottom: 0.5rem;
    color: rgba(255, 255, 255, 0.8);
}

.involvement-list {
    list-style: none;
    padding: 0;
    margin: 1.5rem 0;
}

.involvement-list li {
    margin-bottom: 0.8rem;
    padding-left: 1.5rem;
    position: relative;
    color: rgba(255, 255, 255, 0.9);
}

.involvement-list li::before {
    content: '→';
    position: absolute;
    left: 0;
    color: var(--accent-color);
}

.social-links {
    display: flex;
    gap: 1.5rem;
    margin-top: 1.5rem;
}

.social-link {
    color: var(--text-color);
    text-decoration: none;
    font-family: var(--heading-font);
    font-size: 0.9rem;
    text-transform: uppercase;
    letter-spacing: 1px;
    transition: color 0.3s ease;
}

.social-link:hover {
    color: var(--accent-color);
}

@media (max-width: 768px) {
    .about-title {
        font-size: 2rem;
    }

    .topics-grid {
        grid-template-columns: 1fr;
    }

    .about-section h2 {
        font-size: 1.5rem;
    }
}
</style>
