<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AR Portfolio</title>
    <link rel="stylesheet" href="endsem.css">

   <style>
        body {
    margin: 0;
    font-family: Arial;
    background-color: #FFFFFF;
}

.container {
    width: 1440px;

    
  padding:20px;
    box-sizing: border-box;
}

.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    justify-content: center;
    margin-left: 135px;
    width: 1080px;
    height: 72px;
    padding: 0 20px;
    background: rgba(51, 51, 51, 0.08);
    border-radius: 20px;
}

.logo {
    flex-grow: 1;
    text-align: center;
    
}

.logo h1 {
    font-size: 42px;
    font-family: 'Bebas Neue', monospace;
    color: #000;
    margin: 0;
    text-align: center;
    align-items: center;
    margin-right: 100px;
}

.page-links {
    display: flex;
    gap: 40px;
    

}

.page-links a {
    text-decoration: none;
    color: #000;
   gap: 20px;
    font-size: 17px;
    line-height: 24px;
    font-family:'Roboto Mono', monospace;
;
}

.landing-hero {
    margin-top: 20px;
    text-align: center;
    font-size: 60px;
    font-family: 'Bebas Neue', monospace;

}

.landing-hero img {
    width: 1344px;
    height: 672px;
    object-fit: cover;
}

.about-section {
    margin-top: 20px;
    font-size: 60px;
    font-weight: 400;
    line-height: 68px;
    align-items: left;
    text-align: left;
    font-family: 'Bebas Neue', monospace;

}

.designer-image {
    margin-top: 20px;
    text-align: left;
}

.designer-image img {
    width: 1400px;
    height: 810px;
    object-fit: cover;
}


.project-overview {
    margin-top: 40px;
    text-align: left;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    gap: 10px;
}

.project {
    flex: 1;
    min-width: 300px;
    margin-bottom: 40px;
    font-family:'Roboto Mono', monospace;
}

.project img {
    width: 417px;
    height: 277px;
    object-fit: cover;
    
}

.testimonials-section {
    width: 100%;
    text-align: center;
    margin: 48px 0;
}

.testimonials-section h2 {
    font-family: 'Bebas Neue', monospace;
    font-size: 32px;
    color: #000;
    margin-bottom: 24px;
}

.comment-section {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    width: 100%;
    max-width: 1200px;
    margin: 20px auto;
    padding: 10px;
 
}

.comment {
    display: flex;
    align-items: flex-start;
    width: 22%;
    margin-bottom: 20px;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 10px;
    background-color: #fff;
    font-family:'Roboto Mono', monospace;
}

.comment-photo {
    width: 48px;
    height: 48px;
    border-radius: 50%;
    object-fit: cover;
    margin-right: 10px;
}

.comment-content {
    flex: 1;
    font-family:'Roboto Mono', monospace;
}

.comment-name {
  font-size: 15px;
  text-align: left;
    display: block;
    margin-bottom: 5px;
    font-family:'Roboto Mono', monospace;
}

.comment-text {
    margin: 0;
    text-align: left;
    font-size: 20px;
    font-family:'Roboto Mono', monospace;
}

/* Separator line */
.separator-line {
    width: 1536px;
    height: 1px;
    background-color: #000;
    margin:0px ;
    padding:0px;
    
}

.impact-section {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    padding: 48px 0;
    gap: 48px;
    width: 1344px;
    height: 408px;
    background: #FFFFFF;
    z-index: 0;
    margin-top: 40px;

    

}

.impact-header {
    height: 32px;
    font-size: 28px;
    line-height: 32px;
    letter-spacing: -0.01em;
    color: #000000;
    margin-left: 50px;
    margin-right: 10px;
    font-family: 'Bebas Neue', monospace;
}

.impact-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 30px;
    margin-left: 550px;
}

.impact-item {
    text-align: left;
    position: relative;
    width: 250px;
}

.impact-item::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 1px;
    background-color: #000000;
}

.impact-number {
    font-size: 48px;
    font-weight: 400;
    font-family: 'Bebas Neue', monospace;

}

.impact-text {
    font-size: 20px;
    font-family:'Roboto Mono', monospace;
}

.footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
   
    
    width: 100%;
}

.footer-left {
    display: flex;
    align-items: center;
    gap: 10px;
    font-weight: bold;
    font-family: 'Bebas Neue', monospace;

}

.footer-left .circle {
    width: 30px;
    height: 30px;
    border-radius: 50%;
    background-color: transparent;
    border: 2px solid #000;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 18px;
    color: #000;
    
}

.footer-right {
    display: flex;
    justify-content: flex-end;
    
}

.footer-right .contact-box {
    width: 169px;
    height: 48px;
    border-radius: 8px;
    border: 2px solid #000;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 20px;
    color: #000;
    padding: 0 20px;
    font-family:'Roboto Mono', monospace;
}

.footer-right .contact-box a {

  color: #000;
}

.footer p {
    font-family: Arial, sans-serif;
    font-size: 14px;
    color: #000;
    margin: 0;
}

.footer-links {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin-top: 8px;
}

.footer-links a {
    
  color: #000;
    font-family: 'Arial', sans-serif;
    font-size: 14px;
}



/* Media Queries for Responsiveness */

/* For screens smaller than 1200px (to adjust for 13-inch MacBook) */
@media (max-width: 1200px) {
    .container {
        padding: 15px;
    }

  .header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        justify-content: center;
        margin-left: 135px;
        width: 1080px;
        height: 72px;
        padding: 0 20px;
        background: rgba(51, 51, 51, 0.08);
        border-radius: 20px;
    }

  .logo h1 {
        font-size: 36px;
    }

  .landing-hero h2 {
        font-size: 48px;
    }

  .project-overview {
        justify-content: space-around;
    }

   .impact-grid {
        grid-template-columns: 1fr 1fr;
        margin-left: 0;
    }

  .impact-header {
        text-align: center;
    }

   .impact-item {
        width: 100%;
    }

   .footer {
        flex-direction: column;
        text-align: center;
    }

  .footer-left {
        margin-bottom: 20px;
    }
}

/* For screens smaller than 768px */
@media (max-width: 769px) {
    .header {
        padding: 10px;
        display: flex;
    justify-content: space-between;
    align-items: center;
    justify-content: center;
    }

  .logo h1 {
        font-size: 28px;
    }

  .page-links {
        flex-direction: column;
        gap: 10px;
        font-size: 14px;
    }

   .landing-hero h2 {
        font-size: 28px;
    }

   .impact-header {
        font-size: 24px;
    }

  .impact-item {
        width: 100%;
    }

  .footer {
        flex-direction: column;
        text-align: center;
    }

  .footer-right .contact-box {
        width: 100%;
    }

   .project img {
        width: 90%; /* Smaller images for mobile */
        max-width: 250px;
    }

  .comment {
        width: 100%;
        margin-bottom: 10px;
    }

   .comment-text {
        font-size: 16px;
    }
}

/* For screens smaller than 480px */
@media (max-width: 480px) {
    .header {
        padding: 10px;
        display: flex;
    justify-content: space-between;
    align-items: center;
    justify-content: center;
    }
    .logo h1 {
        font-size: 24px;
    }

.page-links {
        flex-direction: column;
        gap: 10px;
        font-size: 12px;
    }

  .landing-hero h2 {
        font-size: 22px;
    }

   .impact-section {
        flex-direction: column;
        align-items: center;
        gap: 20px;
    }

.impact-grid {
        grid-template-columns: 1fr;
        margin-left: 0;
    }

  .footer {
        flex-direction: column;
        text-align: center;
    }

   .footer-right .contact-box {
        width: 100%;
    }

   .project img {
        width: 100%;
        max-width: 200px;
    }

   .comment {
        width: 100%;
    }

   .comment-name {
        font-size: 12px;
    }

   .comment-text {
        font-size: 14px;
    }
}
</style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="page-links">
                <a href="#">Home</a>
                <a href="#">Projects</a>
                <a href="#">About</a>
            </div>
            <div class="logo">
                <h1>ARFOLIO</h1>
            </div>
            <div class="socials">
                <a style="text-decoration: none;
                color: #000;font-family:'Roboto Mono', monospace;
                ;font-size: 16px;" href="#" >Contact</a>
            </div>
        </div>
        <div class="landing-hero">
            <h2>BRIDGING DIGITAL AND PHYSICAL DESIGN</h2>
            <img src="1.jpeg" alt="Hero Image">
        </div>
        <div class="about-section">
            <p>Innovative designer blending AR with traditional aesthetics. Part digital, part physical, always cutting-edge.</p>
        </div>
        <div class="designer-image">
            <img src="2.jpeg" alt="Designer Image">
        </div>
        <div class="project-overview">
            <div class="row">
                <div class="project">
                    <img src="3.jpeg" alt="Project Image">
                    <p style=" margin-top:20px;">Holographic Branding</p>
                    <p style="font-size: 14px;">AR Design</p>
                </div>
                <div class="project">
                    <img src="4.jpeg" alt="Project Image">
                    <p style=" margin-top:20px;">Virtual Reality Spaces</p>
                    <p style="font-size: 14px;">VR Design</p>
                </div>
                <div class="project">
                    <img src="5.jpeg" alt="Project Image">
                    <p style=" margin-top:20px;">Digital Sculpture</p>
                    <p style="font-size: 14px;">3D Art</p>
                </div>
            </div>
            <div class="row">
                <div class="project">
                    <img src="6.jpeg" alt="Project Image">
                    <p style=" margin-top:20px;">Interactive Installations</p>
                    <p style="font-size: 14px;">Experiential Design</p>
                </div>
                <div class="project">
                    <img src="7.jpeg" alt="Project Image">
                    <p style=" margin-top:20px;">Augmented Interiors</p>
                    <p style="font-size: 14px;">Interior Design</p>
                </div>
                <div class="project">
                    <img src="8.jpeg" alt="Project Image">
                    <p style=" margin-top:20px;">Mixed Reality Exhibits</p>
                    <p style="font-size: 14px;">Exhibit Design</p>
                </div>
            </div>
            <div class="row">
                <div class="project">
                    <img src="9.jpeg" alt="Project Image">
                    <p style=" margin-top:20px;">Virtual Fashion</p>
                    <p style="font-size: 14px;">Fashion Design</p>
                </div>
                <div class="project">
                    <img src="10.jpeg" alt="Project Image">
                    <p style=" margin-top:20px;">3D Printed Art</p>
                    <p style="font-size: 14px;">Sculpture</p>
                </div>
                <div class="project">
                    <img src="11.jpeg" alt="Project Image">
                    <p style=" margin-top:20px;">HoloLens Prototypes</p>
                    <p style="font-size: 14px;">Prototyping</p>
                </div>
            </div>
        </div>
        <div class="testimonials-section">
            <h2>What Our Clients Say</h2>
            <div class="comment-section">
                <div class="comment">
                    <img class="comment-photo" src="12.jpeg" alt="Commenter Photo">
                    <div class="comment-content">
                        <span class="comment-name">Aurelia F.   </span>
                        <span class="comment-name">Creative Director, Future Visions</span>
                        <div class="comment-line"></div>
                        <p class="comment-text">A revolutionary approach to design.</p>
                    </div>
                </div>
                <div class="comment">
                    <img class="comment-photo" src="13.jpeg" alt="Commenter Photo">
                    <div class="comment-content">
                        <span class="comment-name">Leona R.</span>
                        <span class="comment-name">Founder, ArtSpace</span>
                        <div class="comment-line"></div>
                        <p class="comment-text">Transformed our brand with AR.</p>
                    </div>
                </div>
                <div class="comment">
                    <img class="comment-photo" src="14.jpeg" alt="Commenter Photo">
                    <div class="comment-content">
                        <span class="comment-name">Darius T.</span>
                        <span class="comment-name">Head of Design, Immersive Worlds</span>
                        <div class="comment-line"></div>
                        <p class="comment-text">Pioneering work in mixed reality.</p>
                    </div>
                </div>
                <div class="comment">
                    <img class="comment-photo" src="15.jpeg" alt="Commenter Photo">
                    <div class="comment-content">
                        <span class="comment-name">Aurelia F.   </span>
                        <span class="comment-name">CEO, Tech Innovators</span>
                        <div class="comment-line"></div>
                        <p class="comment-text">Exceptional design and execution.</p>
                    </div>
                </div>
            </div>
        </div>
        <!-- Full-width line -->
        <div  class="separator-line"></div>
        <div class="impact-section">
            <div style="margin-right:175px ; font-style: 
Bebas Neue;" class="impact-header">Our Impact</div>
            <div class="impact-grid">
                <div class="impact-item">
                    <div class="impact-number">150+</div>
                    <div class="impact-text">Projects Completed</div>
                </div>
                <div class="impact-item">
                    <div class="impact-number">50+</div>
                    <div class="impact-text">Satisfied Clients</div>
                </div>
                <div class="impact-item">
                    <div class="impact-number">10</div>
                    <div class="impact-text">Years of Experience</div>
                </div>
                <div class="impact-item">
                    <div class="impact-number">5</div>
                    <div class="impact-text">Industry Awards</div>
                </div>
            </div>
        </div>
        <div class="footer">
            <div class="footer-left">
                <div class="circle">©</div>
                <p>2024 ARFOLIO. All rights reserved.</p>
            </div>
            <div class="footer-right">
                <div class="contact-box">
                    <a href="#">Contact Us</a>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
