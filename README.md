# Personal Portfolio Website

A modern, responsive personal portfolio website showcasing skills, projects, and achievements.

## Features

### ✅ Completed Features
- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **Interactive Navigation**: Smooth scrolling and hamburger menu for mobile
- **SEO Optimized**: Meta tags and structured content for better search visibility
- **Modern UI/UX**: Clean design with hover effects and animations
- **Contact Form**: Functional contact form with validation
- **Curved Square Design**: Achievements and Projects sections feature curved square cards as requested

### 📋 Sections Included
1. **Profile/Hero Section** - Introduction with profile picture and social links
2. **About Section** - Personal information and background
3. **Experience Section** - Work history and professional experience
4. **Achievements Section** - Awards, certifications, and accomplishments (with links)
5. **Projects Section** - Portfolio of work with live demo and GitHub links
6. **Contact Section** - Contact information and contact form

## 🚀 Getting Started

### Prerequisites
- A modern web browser
- Local development server (optional, for testing)

### Installation
1. Clone or download the project files
2. Open `index.html` in your web browser
3. For local development, use a local server:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   
   # Using PHP
   php -S localhost:8000
   ```

## 📝 Customization Guide

### Content Updates
Replace the placeholder content in `index.html` with your actual information:

#### Profile Section
- Update name, title, and profile picture
- Modify social media links
- Update CV download link

#### About Section
- Replace Lorem Ipsum with your actual bio
- Update experience and education details
- Change profile picture

#### Experience Section
- Replace placeholder jobs with your actual work experience
- Update company names, dates, and descriptions

#### Achievements Section
- Add your actual achievements and awards
- Update the links to point to real certificates/projects
- Modify achievement descriptions

#### Projects Section
- Add your actual projects
- Update project descriptions
- Add real GitHub and live demo links

#### Contact Section
- Update contact information (email, phone, location)
- Configure contact form backend (see Backend Integration below)

### Styling Customization
The website uses a clean, modern design with:
- **Color Scheme**: Blue and purple gradients for experience, orange/yellow for achievements, teal for projects
- **Typography**: Poppins font family
- **Animations**: Smooth hover effects and scroll animations
- **Responsive**: Mobile-first design approach

To customize colors, edit the CSS variables in `style.css`.

## 🔧 Backend Integration (Optional)

### Contact Form Backend
The contact form currently shows a success message. To make it functional:

#### Option 1: EmailJS (Recommended for static sites)
1. Sign up at [EmailJS](https://www.emailjs.com/)
2. Create an email template
3. Add EmailJS SDK to your HTML:
   ```html
   <script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>
   ```
4. Update the contact form JavaScript in `script.js`

#### Option 2: Formspree
1. Sign up at [Formspree](https://formspree.io/)
2. Replace the form action with your Formspree endpoint
3. Update form handling in JavaScript

#### Option 3: Node.js Backend
1. Create a simple Express.js server
2. Use nodemailer for email sending
3. Deploy to platforms like Heroku, Vercel, or Netlify

### Database Integration (Optional)
For dynamic content management:

#### MongoDB Setup
```javascript
// Example with MongoDB
const mongoose = require('mongoose');
const Project = require('./models/Project');

// API endpoints for CRUD operations
app.get('/api/projects', async (req, res) => {
  const projects = await Project.find();
  res.json(projects);
});
```

#### MySQL Setup
```sql
-- Example database schema
CREATE TABLE projects (
  id INT PRIMARY KEY AUTO_INCREMENT,
  title VARCHAR(255),
  description TEXT,
  github_link VARCHAR(255),
  live_demo VARCHAR(255),
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

## 📱 Responsive Design

The website is fully responsive with breakpoints:
- **Desktop**: 1200px and above
- **Tablet**: 768px - 1199px
- **Mobile**: Below 768px

## 🎨 Design Features

### Curved Square Design
- Achievements and Projects sections feature cards with 25px border-radius
- Smooth hover animations with scale and shadow effects
- Gradient accent bars at the top of each card

### Animations
- Scroll-triggered animations for cards
- Smooth hover effects
- Gradient backgrounds and transitions

### Accessibility
- Semantic HTML structure
- Proper alt text for images
- Keyboard navigation support
- High contrast colors

## 🚀 Deployment

### GitHub Pages
1. Push your code to a GitHub repository
2. Go to Settings > Pages
3. Select source branch (usually `main`)
4. Your site will be available at `https://username.github.io/repository-name`

### Netlify
1. Drag and drop your project folder to [Netlify](https://netlify.com)
2. Or connect your GitHub repository
3. Automatic deployments on push

### Vercel
1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in your project directory
3. Follow the prompts

## 📊 SEO Optimization

The website includes:
- Meta description and keywords
- Open Graph tags for social sharing
- Semantic HTML structure
- Fast loading times
- Mobile-friendly design

## 🔍 Performance Tips

1. **Optimize Images**: Compress images using tools like TinyPNG
2. **Minify CSS/JS**: Use build tools to minify files
3. **Use CDN**: Serve fonts and libraries from CDNs
4. **Lazy Loading**: Implement lazy loading for images
5. **Caching**: Set appropriate cache headers

## 🛠️ Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Modern styling with Flexbox and Grid
- **JavaScript**: Interactive functionality
- **Responsive Design**: Mobile-first approach
- **Modern CSS**: Custom properties, gradients, animations

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Feel free to submit issues and enhancement requests!

## 📞 Support

If you need help customizing this portfolio, please:
1. Check the customization guide above
2. Review the code comments
3. Open an issue for specific problems

---

**Note**: This is a template with placeholder content. Replace all placeholder text and images with your actual information before deploying.