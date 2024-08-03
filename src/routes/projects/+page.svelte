<script>
    // Your existing script content (if any)
    const projects = [
    {
      title: "Project 1",
      description: "Short description of Project 1",
      link: "https://github.com/yourusername/project1"
    },
    {
      title: "Project 2",
      description: "Short description of Project 2",
      link: "https://github.com/yourusername/project2"
    },
    {
      title: "Project 3",
      description: "Short description of Project 3",
      link: "https://github.com/yourusername/project3"
    }
  ];
  </script>
  
  <section class="projects">
    {#each projects as project}
      <div class="project-card">
        <h2>{project.title}</h2>
        <p>{project.description}</p>
        <a href={project.link} target="_blank" rel="noopener noreferrer">View on GitHub</a>
      </div>
    {/each}
  </section>

  <div class="github-graph-container">
    <img src="https://ghchart.rshah.org/andrewalson" alt="@andrewalson's Github calendar" class="github-graph" />
  </div>

  <style>
    .projects {
    display: flex;
    flex-direction: column;
    gap: 20px;
    margin-bottom: 40px;
    width: 90%;
    align-items: center;
    /*justify-content: space-between;*/
  }

  .project-card {
    background-color: #f0f0f0;
    border-radius: 8px;
    padding: 15px;
    flex: 1;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 120px; /* Adjust this value to make cards shorter or taller */
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease;
  }

  .project-card:hover {
    transform: translateY(-5px);
  }

  .project-card h2 {
    margin: 0;
    font-size: 1rem;
    color: #333;
  }

  .project-card p {
    margin: 5px 0;
    font-size: 0.8rem;
    color: #666;
    flex-grow: 1;
  }

  .project-card a {
    font-size: 0.8rem;
    color: #0066cc;
    text-decoration: none;
    align-self: flex-start;
  }

  .project-card a:hover {
    text-decoration: underline;
  }

  .github-graph-container {
    width: 100%;
    position: relative;
    padding-top: 10px;
  }

  .github-graph {
    position: absolute;
    max-width: none;
  }

  @media (max-width: 768px) {
    .projects {
      flex-direction: column;
    }
  }

  @media (max-width: 480px) {
    .project-card {
      height: auto;
      padding: 10px;
    }
  }

  </style>