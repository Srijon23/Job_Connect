# JobConnect - Job Portal System

A comprehensive job portal platform connecting job seekers with employers, featuring advanced search capabilities, application tracking, and profile management.

## Features

### For Job Seekers
- User registration and authentication
- Create and manage professional profiles
- Advanced job search with filters (location, salary, category, etc.)
- Apply to jobs with resume uploads
- Track application status
- Save favorite job listings
- Receive job recommendations

### For Employers
- Company profile creation
- Post and manage job listings
- Review candidate applications
- Search candidate database
- Applicant tracking system
- Interview scheduling

### General Features
- Responsive design for mobile and desktop
- Real-time notifications
- Secure authentication
- Admin dashboard for platform management
- Email notifications

## Technologies Used

### Frontend
- HTML5, CSS3, JavaScript
- Bootstrap (responsive UI)
- jQuery (DOM manipulation)

### Backend
- PHP (server-side logic)
- MySQL (database)

### Additional Tools
- PHPMailer (email notifications)
- PDF generation libraries
- File upload handling

## Installation

### Prerequisites
- XAMPP/WAMP/LAMP server (Apache + MySQL + PHP 7.4+)
- Web browser
- Text editor (VS Code, Sublime, etc.)

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/Srijon23/Job_Connect.git
   cd Job_Connect
   ```

2. **Start your local server**
   - Start Apache and MySQL from XAMPP/WAMP control panel

3. **Create database**
   - Open phpMyAdmin (http://localhost/phpmyadmin)
   - Create a new database named `job_portal`
   - Import the SQL file: `database/job_portal.sql`

4. **Configure database connection**
   - Open `config/database.php` or relevant config file
   - Update database credentials:
     ```php
     $host = "localhost";
     $username = "root";
     $password = "";
     $database = "job_portal";
     ```

5. **Set up file permissions**
   - Ensure uploads directory is writable:
     ```bash
     chmod 755 uploads/
     ```

6. **Access the application**
   - Open browser and navigate to: `http://localhost/Job_Connect`

## Project Structure

```
Job_Connect/
├── assets/
│   ├── css/          # Stylesheets
│   ├── js/           # JavaScript files
│   └── images/       # Images and icons
├── config/
│   └── database.php  # Database configuration
├── includes/
│   ├── header.php    # Common header
│   └── footer.php    # Common footer
├── uploads/
│   ├── resumes/      # Uploaded resumes
│   └── profiles/     # Profile pictures
├── admin/            # Admin panel
├── employer/         # Employer dashboard
├── jobseeker/        # Job seeker dashboard
├── database/         # SQL files
├── index.php         # Landing page
└── README.md
```

## Usage

### Job Seekers
1. Register as a job seeker
2. Complete your profile with skills and experience
3. Upload your resume
4. Search for jobs using filters
5. Apply to relevant positions
6. Track your applications

### Employers
1. Register as an employer
2. Create company profile
3. Post job openings
4. Review applications
5. Contact candidates
6. Manage job listings

### Admin
1. Login with admin credentials
2. Manage users (job seekers and employers)
3. Moderate job postings
4. View platform analytics
5. Handle reported content

## Default Credentials

**Admin:**
- Username: `admin`
- Password: `admin123`

**Test Employer:**
- Email: `employer@test.com`
- Password: `test123`

**Test Job Seeker:**
- Email: `jobseeker@test.com`
- Password: `test123`

*(Change these credentials after first login)*

## Security Features

- Password hashing (bcrypt)
- SQL injection prevention (prepared statements)
- XSS protection
- CSRF token validation
- Session management
- File upload validation

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

## Known Issues

- Email notifications may require SMTP configuration
- PDF generation might need additional PHP extensions

## Future Enhancements

- [ ] AI-powered job recommendations
- [ ] Video interview integration
- [ ] Advanced analytics dashboard
- [ ] Mobile application
- [ ] Social media integration
- [ ] Chat system between employers and candidates

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

**Developer:** Srijon
**GitHub:** [@Srijon23](https://github.com/Srijon23)
**Project Link:** [https://github.com/Srijon23/Job_Connect](https://github.com/Srijon23/Job_Connect)

## Acknowledgments

- Bootstrap for responsive UI components
- Font Awesome for icons
- PHP community for resources and support

---

⭐ If you find this project helpful, please consider giving it a star on GitHub!
