# Mo Soft Solutions

**Professional Software Development Services**

A modern, premium freelancing website showcasing software development services including e-commerce platforms, websites, web applications, and SaaS solutions.

![Mo Soft Solutions](./assets/logo.png)

## 🚀 Live Demo

Visit the live website: [Mo Soft Solutions](#) *(Add your GitHub Pages URL here)*

## 📋 About

Mo Soft Solutions specializes in creating powerful software solutions that transform businesses. We offer:

- **E-Commerce Platforms** - Custom online stores with secure payment integration
- **Business Websites & Web Apps** - Professional, responsive websites
- **SaaS Solutions** - Scalable cloud-based platforms
- **Custom Software Development** - Tailored solutions for unique business needs

## 🛠️ Technologies Used

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Design**: Glassmorphism, Dark Theme, Gradient Accents
- **Features**: Smooth Scrolling, Animated Counters, Responsive Design
- **Form Handling**: Formspree Integration

## 📦 Project Structure

```
MoSoftSolutions/
├── index.html          # Main HTML file
├── style.css           # Premium CSS styling
├── script.js           # Interactive JavaScript
├── assets/             # Images and resources
│   ├── logo.png
│   ├── ecommerce.png
│   ├── website.png
│   └── saas.png
└── README.md           # This file
```

## 🌐 GitHub Pages Deployment

### Option 1: Deploy from Main Branch

1. **Push to GitHub**:

   ```bash
   cd MoSoftSolutions
   git init
   git add .
   git commit -m "Initial commit: Mo Soft Solutions website"
   git branch -M main
   git remote add origin https://github.com/ngwanatuka/MoSoftSolutions.git
   git push -u origin main
   ```

2. **Enable GitHub Pages**:
   - Go to your repository on GitHub
   - Click **Settings** → **Pages**
   - Under "Source", select **main** branch
   - Select **/ (root)** folder
   - Click **Save**
   - Your site will be published at: `https://YOUR_USERNAME.github.io/MoSoftSolutions/`

### Option 2: Deploy to a Custom Repository

If you want to use a custom domain or different repository name:

1. Create a new repository on GitHub (e.g., `mosoft-solutions`)
2. Follow the same steps as Option 1
3. Your site will be at: `https://YOUR_USERNAME.github.io/mosoft-solutions/`

### Option 3: Use as Main GitHub Pages Site

To deploy as your main GitHub Pages site (`https://YOUR_USERNAME.github.io`):

1. Create a repository named exactly: `YOUR_USERNAME.github.io`
2. Push the code to this repository
3. The site will automatically be published at: `https://YOUR_USERNAME.github.io`

## 🔧 Local Development

To run the website locally:

1. **Clone the repository**:

   ```bash
   git clone https://github.com/YOUR_USERNAME/MoSoftSolutions.git
   cd MoSoftSolutions
   ```

2. **Open in browser**:
   - Simply open `index.html` in your web browser
   - Or use a local server:

     ```bash
     # Using Python
     python -m http.server 8000
     
     # Using Node.js (http-server)
     npx http-server
     ```

   - Navigate to `http://localhost:8000`

## ✏️ Customization

### Update Contact Information

Edit `index.html` and update:

- Email addresses
- Phone number
- LinkedIn URL
- GitHub URL

### Modify Services

Edit the services section in `index.html` to add/remove/modify service offerings.

### Change Colors

Edit `style.css` CSS variables at the top:

```css
:root {
  --accent-primary: #667eea;
  --accent-secondary: #764ba2;
  /* ... other colors */
}
```

### Update Portfolio Projects

Edit the portfolio section in `index.html` to showcase your actual projects.

### Form Integration

The contact form uses Formspree. To use your own:

1. Sign up at [Formspree.io](https://formspree.io)
2. Create a new form
3. Replace the form action URL in `index.html`:

   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

## 📱 Features

- ✅ Fully Responsive Design
- ✅ Modern Dark Theme with Glassmorphism
- ✅ Smooth Scroll Animations
- ✅ Animated Statistics Counters
- ✅ Interactive Floating Cards
- ✅ Contact Form with Validation
- ✅ Back-to-Top Button
- ✅ Mobile-Friendly Navigation
- ✅ SEO Optimized
- ✅ Fast Loading Performance

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 📞 Contact

**Mo Soft Solutions**

- Email: <ngwanatuka@gmail.com>
- Phone: +27 64 795 8934
- LinkedIn: [Ngwanatuka Molepo](https://www.linkedin.com/in/ngwanatuka-molepo-75b499259)
- GitHub: [@Ngwanatuka](https://github.com/Ngwanatuka)

---

**Built with ❤️ by Mo Soft Solutions**
