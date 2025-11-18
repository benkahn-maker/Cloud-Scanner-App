# Cloud Security Scanner

![Cloud Security Scanner](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Node](https://img.shields.io/badge/node-%3E%3D18.0.0-brightgreen)

A comprehensive cloud security scanner that detects vulnerabilities, malware, and misconfigurations across AWS, Azure, and GCP infrastructure.

## 🚀 Features

- **Multi-Cloud Support**: AWS, Azure, GCP
- **OWASP Top 10 Coverage**: Complete coverage of all OWASP 2021 categories
- **Real-time Scanning**: Actual cloud resource scanning with credential validation
- **Comprehensive Detection**:
  - Malware detection
  - Vulnerability scanning
  - Security misconfigurations
  - Broken access control
  - Cryptographic failures
  - Injection vulnerabilities
  - And more...
- **Professional GUI**: Modern, responsive interface with detailed findings
- **Actionable Recommendations**: Clear remediation steps for each finding

## 🛠️ Tech Stack

**Frontend:**
- React 18
- Tailwind CSS
- Lucide React (Icons)

**Backend:**
- Node.js + Express
- AWS SDK v3
- Azure SDK
- Google Cloud SDK

## 📋 Prerequisites

- Node.js >= 18.0.0
- npm >= 8.0.0
- Valid cloud provider credentials (AWS/Azure/GCP)

## 🔧 Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/cloud-security-scanner.git
cd cloud-security-scanner
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment (optional)

Create a `.env` file in the root directory:

```env
PORT=3001
NODE_ENV=development
```

## 🚀 Running the Application

### Development Mode (Recommended)

Run both frontend and backend simultaneously:

```bash
npm run dev
```

This will start:
- **Backend**: http://localhost:3001
- **Frontend**: http://localhost:3000

### Production Mode

Build the frontend:

```bash
npm run build
```

Run the backend:

```bash
npm run backend
```

Serve the built frontend with a static server or deploy to your hosting platform.

## 📖 Usage

### 1. Start the Application

```bash
npm run dev
```

### 2. Configure Cloud Provider

Navigate to the **Configuration** tab and enter your credentials:

**For AWS:**
- Access Key ID
- Secret Access Key
- Region (e.g., us-east-1)

**For Azure:**
- Client ID
- Client Secret
- Tenant ID
- Subscription ID

**For GCP:**
- Project ID
- Service Account Credentials (JSON)

### 3. Select Resources to Scan

Choose which resource types to scan:
- ✅ Object Storage (S3, Blob, Cloud Storage)
- ✅ Serverless Functions (Lambda, Functions, Cloud Functions)
- ✅ Compute Instances (EC2, VM, Compute Engine)
- ✅ Managed Databases (RDS, SQL Database, Cloud SQL)
- ✅ Container Orchestration (EKS, AKS, GKE)
- ✅ Network & Security

### 4. Run the Scan

Click **"Start Security Scan"** and wait for results.

### 5. Review Findings

- View detailed findings organized by severity
- See OWASP Top 10 coverage
- Get actionable remediation recommendations
- Export reports for compliance

## 🔒 Security

### Credential Handling

- **Encryption**: All credentials are encrypted with AES-256
- **No Storage**: Credentials are not stored after scanning
- **Validation**: Real-time credential validation before scanning
- **Scope**: Used exclusively for scan execution

### Important Security Notes

⚠️ **Never commit credentials to the repository**
⚠️ **Always use environment variables or secure secret management**
⚠️ **Follow principle of least privilege for cloud credentials**

## 📊 OWASP Top 10 2021 Coverage

The scanner detects vulnerabilities across all OWASP Top 10 categories:

| Category | Description | Examples |
|----------|-------------|----------|
| **A01:2021** | Broken Access Control | Public S3 buckets, overly permissive IAM |
| **A02:2021** | Cryptographic Failures | Unencrypted storage, weak encryption |
| **A03:2021** | Injection | SQL injection, command injection |
| **A04:2021** | Insecure Design | Missing rate limiting, poor architecture |
| **A05:2021** | Security Misconfiguration | Default configs, open ports |
| **A06:2021** | Vulnerable Components | Outdated packages, known CVEs |
| **A07:2021** | Authentication Failures | Missing MFA, weak passwords |
| **A08:2021** | Data Integrity Failures | Supply chain attacks, malware |
| **A09:2021** | Logging Failures | Missing logs, no monitoring |
| **A10:2021** | SSRF | Server-side request forgery |

## 🏗️ Project Structure

```
cloud-security-scanner/
├── public/
│   └── index.html          # HTML template
├── src/
│   ├── App.js              # Main React component
│   ├── index.js            # React entry point
│   └── index.css           # Global styles
├── server.js               # Express backend server
├── package.json            # Dependencies and scripts
├── .gitignore              # Git ignore rules
├── .env.example            # Environment variables template
└── README.md               # This file
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### Development Guidelines

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🐛 Known Issues & Limitations

- Azure and GCP scanning are partially implemented
- Container scanning requires additional permissions
- Large-scale scans may take several minutes
- Rate limiting applies to cloud provider APIs

## 🔮 Roadmap

- [ ] Complete Azure and GCP implementation
- [ ] Add Kubernetes security scanning
- [ ] Implement compliance frameworks (PCI-DSS, HIPAA, SOC2)
- [ ] Add scheduled scanning
- [ ] Email notifications for critical findings
- [ ] Integration with SIEM systems
- [ ] PDF report generation
- [ ] Multi-account support
- [ ] Historical scan comparison

## 📞 Support

For issues, questions, or contributions:
- Open an issue on GitHub
- Contact: your-email@example.com

## 🙏 Acknowledgments

- Built with [React](https://reactjs.org/)
- Icons by [Lucide](https://lucide.dev/)
- Styled with [Tailwind CSS](https://tailwindcss.com/)
- Cloud SDKs by AWS, Azure, and Google Cloud

---

**⚠️ Disclaimer**: This tool is for authorized security testing only. Always ensure you have permission before scanning cloud infrastructure. Unauthorized scanning may violate terms of service and laws.

**Made with ❤️ for cloud security**
