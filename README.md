# Ramesh Maneddi - Portfolio Website

A modern, responsive portfolio website built with Spring Boot, Thymeleaf, and Bootstrap. This application showcases my professional experience, skills, and projects as a Java Backend Developer.

## 🚀 Features

- **Responsive Design**: Optimized for both desktop and mobile devices
- **Modern UI/UX**: Clean, professional design with smooth animations
- **Interactive Elements**: Skill progress bars, floating cards, and hover effects
- **Contact Form**: Functional contact form with validation
- **Social Integration**: Links to LinkedIn, GitHub, and WhatsApp
- **SEO Optimized**: Proper meta tags and semantic HTML structure
- **Docker Support**: Containerized application for easy deployment

## 🛠️ Technology Stack

- **Backend**: Java 17, Spring Boot 3.2.0
- **Frontend**: Thymeleaf, Bootstrap 5.3.0, HTML5, CSS3, JavaScript
- **Build Tool**: Maven
- **Containerization**: Docker & Docker Compose
- **Icons**: Font Awesome 6.4.0
- **Fonts**: Google Fonts (Poppins)

## 📋 Prerequisites

- Java 17 or higher
- Maven 3.6+
- Docker (optional, for containerized deployment)
- Git

## 🏃‍♂️ Running the Application

### Local Development

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd portfolio-app
   ```

2. **Run with Maven**
   ```bash
   ./mvnw spring-boot:run
   ```
   
   Or on Windows:
   ```cmd
   mvnw.cmd spring-boot:run
   ```

3. **Access the application**
   - Open your browser and navigate to: `http://localhost:8080`

### Production Build

1. **Build the JAR file**
   ```bash
   ./mvnw clean package
   ```

2. **Run the JAR file**
   ```bash
   java -jar target/portfolio-0.0.1-SNAPSHOT.jar
   ```

## 🐳 Docker Deployment

### Using Docker

1. **Build the Docker image**
   ```bash
   docker build -t ramesh-portfolio .
   ```

2. **Run the container**
   ```bash
   docker run -p 8080:8080 ramesh-portfolio
   ```

### Using Docker Compose

1. **Start the application**
   ```bash
   docker-compose up -d
   ```

2. **Stop the application**
   ```bash
   docker-compose down
   ```

3. **View logs**
   ```bash
   docker-compose logs -f portfolio-app
   ```

### Production Deployment with Nginx

For production deployment with SSL and reverse proxy:

```bash
docker-compose --profile production up -d
```

## 📁 Project Structure

```
portfolio-app/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/ramesh/portfolio/
│   │   │       ├── PortfolioApplication.java
│   │   │       └── controller/
│   │   │           └── PortfolioController.java
│   │   └── resources/
│   │       ├── static/
│   │       │   ├── css/
│   │       │   │   └── style.css
│   │       │   ├── js/
│   │       │   │   └── script.js
│   │       │   └── images/
│   │       ├── templates/
│   │       │   ├── index.html
│   │       │   ├── about.html
│   │       │   ├── skills.html
│   │       │   ├── projects.html
│   │       │   └── contact.html
│   │       └── application.properties
│   └── test/
├── Dockerfile
├── docker-compose.yml
├── pom.xml
└── README.md
```

## 🎨 Pages Overview

### Home Page (`/`)
- Hero section with animated introduction
- Quick stats and achievements
- Call-to-action buttons
- Floating skill cards

### About Page (`/about`)
- Professional summary
- Work experience details
- Education background
- Contact information

### Skills Page (`/skills`)
- Interactive skill progress bars
- Categorized technical skills
- Programming languages and frameworks
- Tools and methodologies

### Projects Page (`/projects`)
- Detailed project showcases
- ServicesBay recruitment platform
- Mcafe expense management system
- Technology stacks used

### Contact Page (`/contact`)
- Contact form with validation
- Contact information
- Social media links
- WhatsApp integration

## 🔧 Configuration

### Application Properties

The application can be configured through `application.properties`:

- **Server Configuration**: Port, address, context path
- **Thymeleaf Settings**: Template caching, encoding
- **Logging Configuration**: Log levels, patterns
- **Management Endpoints**: Health checks, monitoring

### Environment Profiles

- **Development** (`dev`): Debug logging, hot reload enabled
- **Production** (`prod`): Optimized settings, security headers

## 🚀 Deployment Options

### Local Development
```bash
./mvnw spring-boot:run -Dspring-boot.run.profiles=dev
```

### Production
```bash
java -jar target/portfolio-0.0.1-SNAPSHOT.jar --spring.profiles.active=prod
```

### Docker Production
```bash
docker run -p 8080:8080 -e SPRING_PROFILES_ACTIVE=prod ramesh-portfolio
```

## 📱 Mobile Responsiveness

The application is fully responsive and optimized for:
- Desktop (1200px+)
- Tablet (768px - 1199px)
- Mobile (320px - 767px)

## 🎯 Performance Features

- **Lazy Loading**: Images and content loaded on demand
- **Caching**: Static resources cached for better performance
- **Compression**: Gzip compression enabled
- **Minification**: CSS and JS optimized for production
- **CDN**: External libraries loaded from CDN

## 🔒 Security Features

- **HTTPS Ready**: SSL/TLS configuration support
- **Security Headers**: XSS protection, content security policy
- **Input Validation**: Form validation and sanitization
- **Session Security**: Secure cookie settings

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Contact

**Ramesh Maneddi**
- Email: rameshmaneddi6@gmail.com
- Phone: +91 8309278773
- LinkedIn: [linkedin.com/in/ramesh-maneddi](https://linkedin.com/in/ramesh-maneddi)
- GitHub: [github.com/ramesh-maneddi](https://github.com/ramesh-maneddi)
- WhatsApp: [wa.me/918309278773](https://wa.me/918309278773)

## 🙏 Acknowledgments

- Spring Boot team for the excellent framework
- Bootstrap team for the responsive CSS framework
- Font Awesome for the beautiful icons
- Google Fonts for the typography

---

**Built with ❤️ by Ramesh Maneddi**

