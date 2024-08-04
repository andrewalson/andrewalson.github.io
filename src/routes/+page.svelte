<script>

   import { base } from "$app/paths";

</script>

<section class="hero">
    <div class="profile-image-container">
      <img src= {'/andrew-calcifer.JPG'} alt="Your Name" class="profile-image">
    </div>
    <div class="hero-content">
      <h1>Andrew Alson</h1>
      <p>Software Engineer studying CS @ WGU based in Raleigh, NC</p>
    </div>
  </section>
  
  <style>
    .hero {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      padding: 2.1rem;
      text-align: center;
    }
  
    .profile-image-container {
      width: 500px;
      height: 500px;
      border-radius: 50%;
      overflow: hidden;
      margin-bottom: .05rem;
      margin-top: 0.8rem;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    }
  
    .profile-image {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
    }
  
    .hero-content {
      margin-top: 0.3rem;
    }
  
    h1 {
      font-size: 2.4rem;
      margin-bottom: 0.5rem;
    }
  
    p {
      font-size: 1.3rem;
      color: #666;
    }
  </style>