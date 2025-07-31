# Rise8 Growth Checklist

<div align="center">
  <h3>🚀 Streamline Your Federal Proposal Development Process</h3>
  <p>A comprehensive task management system designed specifically for government contractors managing multiple concurrent proposals.</p>
  
  ![Version](https://img.shields.io/badge/version-1.0.0-red.svg)
  ![License](https://img.shields.io/badge/license-MIT-blue.svg)
  ![Status](https://img.shields.io/badge/status-active-success.svg)
</div>

---

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Screenshots](#screenshots)
- [Demo](#demo)
- [Quick Start](#quick-start)
- [Usage](#usage)
- [Integrations](#integrations)
- [Technical Details](#technical-details)
- [Deployment](#deployment)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [Support](#support)
- [License](#license)

## 🎯 Overview

The Rise8 Growth Checklist is a powerful web application that helps federal contractors manage the complex proposal development lifecycle. Built with simplicity and efficiency in mind, it provides structured task management, progress tracking, and team coordination features specifically tailored for government contracting.

### Why This Tool?

- **Standardized Process**: Ensures consistent proposal development across all opportunities
- **Multi-Proposal Management**: Track multiple concurrent proposals from a single dashboard
- **Team Coordination**: Assign tasks, set deadlines, and balance workload across team members
- **Integration Ready**: Connects with HubSpot CRM and Slack for seamless workflow integration

## ✨ Features

### Core Functionality

- **📊 Multi-Proposal Dashboard**
  - View all active proposals at a glance
  - Filter by status (Active, Overdue, Completed)
  - Quick statistics and progress tracking
  - One-click access to any checklist

- **✅ Smart Task Management**
  - Pre-configured templates for different proposal types
  - Task assignment to team members
  - Due date tracking with visual urgency indicators
  - Time estimation for resource planning
  - Collapsible sections for better organization

- **🎯 Proposal Templates**
  - Prime Contractor (comprehensive workflow)
  - Subcontractor (streamlined process)
  - SBIR/STTR (research-focused)
  - GSA Schedule (compliance-heavy)
  - Recompete (incumbent advantage)

- **📈 Progress Tracking**
  - Real-time progress bars
  - Task completion statistics
  - Automatic progress calculation
  - Visual indicators for at-risk items

### Advanced Features

- **🔗 HubSpot Integration** (Demo)
  - Create deals automatically
  - Sync progress updates
  - Link to pipeline stages

- **💬 Slack Integration** (Demo)
  - Post new opportunities to channels
  - Thread-based progress updates
  - Team notifications

- **📤 Export Options**
  - Text reports for emails
  - CSV for Excel analysis
  - JSON for data backup
  - All task details included

- **💾 Persistent Storage**
  - Auto-save functionality
  - Browser-based storage
  - No account required
  - Works offline

## 📸 Screenshots

### Dashboard Overview
See all your active proposals at a glance with progress tracking and statistics.

![Dashboard Overview](https://via.placeholder.com/1200x600/1a1a1a/ff0000?text=Dashboard+Overview)

### Creating a New Checklist
Easy setup with proposal templates and integration options.

![New Checklist Form](https://via.placeholder.com/800x600/1a1a1a/ff0000?text=New+Checklist+Form)

### Task Management
Assign tasks, set due dates, and track progress in real-time.

![Active Checklist](https://via.placeholder.com/1200x600/1a1a1a/ff0000?text=Active+Checklist+View)

### Integrations
Seamless connection to HubSpot and Slack for team collaboration.

![Integration Progress](https://via.placeholder.com/600x400/1a1a1a/ff0000?text=Integration+Setup)

### Export Options
Multiple formats for sharing progress reports.

![Export Options](https://via.placeholder.com/600x400/1a1a1a/ff0000?text=Export+Options)

### Mobile Responsive
Full functionality on any device.

<div align="center">
  <img src="https://via.placeholder.com/375x667/1a1a1a/ff0000?text=Mobile+View" alt="Mobile View" width="375">
</div>

## 🚀 Demo

[Live Demo](https://cspakes-rise8.github.io/rise8-checklist) | [Video Walkthrough](#) | [Interactive Tutorial](#)

### Quick Demo Credentials
No login required! The application uses browser storage for persistence.

## 🏃‍♂️ Quick Start

### Option 1: GitHub Pages (Recommended)

1. Fork this repository
2. Enable GitHub Pages in Settings → Pages
3. Select "Deploy from branch" → main → / (root)
4. Access at: `https://cspakes-rise8.github.io/rise8-checklist`

### Option 2: Local Development

```bash
# Clone the repository
git clone https://github.com/cspakes-rise8/rise8-checklist.git

# Navigate to project directory
cd rise8-checklist

# Open in browser (no build process required!)
open index.html

# Or use a local server
python -m http.server 8000
# Visit http://localhost:8000
```

## 📖 Usage

### Creating Your First Checklist

1. **Start from Dashboard**
   - Click "+ New Checklist" button
   - Enter opportunity details
   - Select proposal type
   - Enable integrations (optional)

2. **Manage Tasks**
   - Click checkboxes to complete tasks
   - Assign team members from dropdown
   - Set due dates for each task
   - Adjust time estimates as needed

3. **Track Progress**
   - View overall progress in header
   - Check dashboard for multi-proposal overview
   - Export progress reports anytime

### Working with Templates

Each template includes pre-configured tasks based on proposal type:

```
Prime Contractor (35 tasks)
├── Administration (8 tasks)
├── Partner Coordination (6 tasks)
├── Solution Development (6 tasks)
├── Writing & Review (8 tasks)
├── Pricing (5 tasks)
└── Submission (4 tasks)
```

### Keyboard Shortcuts

- `Tab` - Navigate between controls
- `Space` - Toggle checkbox when focused
- `Enter` - Confirm input changes
- `Esc` - Close modals

## 🔌 Integrations

### HubSpot CRM (Demo Mode)

Configure HubSpot integration during checklist creation:

```javascript
// Example integration payload
{
  "dealName": "DISA Cloud Migration",
  "pipeline": "federal",
  "dealValue": "$5M",
  "stage": "proposal_development"
}
```

### Slack Notifications (Demo Mode)

Post updates to your team channels:

```javascript
// Example Slack message
🚀 New Proposal Checklist Created
Opportunity: DISA Cloud Migration
Type: Prime Contractor
Deadline: March 15, 2024
Total Tasks: 35
```

### API Documentation

For production integration, implement these endpoints:

```
POST /api/hubspot/deals
PUT  /api/hubspot/deals/{dealId}
POST /api/slack/messages
POST /api/slack/threads/{threadTs}/replies
```

## 🛠 Technical Details

### Architecture

```
rise8-checklist/
├── index.html          # Single-file application
├── README.md           # Documentation
└── LICENSE            # MIT License
```

### Technology Stack

- **Frontend**: Vanilla JavaScript (ES6+)
- **Styling**: Custom CSS with CSS Variables
- **Storage**: LocalStorage API
- **Build**: None required (static HTML)
- **Dependencies**: Zero! 🎉

### Browser Support

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers

### Performance

- **Page Load**: < 100ms
- **First Paint**: < 200ms
- **Interactive**: < 300ms
- **Bundle Size**: ~25KB (uncompressed)

## 🚢 Deployment

### GitHub Pages

1. Push code to main branch
2. Enable Pages in repository settings
3. Wait 2-3 minutes for deployment
4. Share your URL!

### Custom Domain

```bash
# Add CNAME file
echo "checklist.rise8.com" > CNAME
git add CNAME
git commit -m "Add custom domain"
git push
```

### Environment Variables

For production integrations, add:

```javascript
// config.js
const CONFIG = {
  HUBSPOT_API_KEY: process.env.HUBSPOT_API_KEY,
  SLACK_BOT_TOKEN: process.env.SLACK_BOT_TOKEN,
  API_ENDPOINT: process.env.API_ENDPOINT || '/api'
};
```

## 🗺 Roadmap

### Version 1.1 (Sprint 2) ✅
- [x] Multi-checklist dashboard
- [x] Task assignments to team members
- [x] Due dates and urgency indicators
- [x] Time estimation per task
- [x] HubSpot & Slack integration (demo)

### Version 1.2 (Sprint 3) - In Progress
- [ ] Team workload visualization
- [ ] Bulk task operations
- [ ] Enhanced filtering options
- [ ] Task dependencies

### Version 1.3 (Q2 2024)
- [ ] Real Google Workspace integration
- [ ] Email notifications
- [ ] Calendar sync
- [ ] Document attachments

### Version 2.0 (Future)
- [ ] Multi-user collaboration
- [ ] Real-time sync
- [ ] Advanced analytics
- [ ] AI-powered insights
- [ ] Mobile app

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md).

### Development Process

1. Fork the repository
2. Create feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open Pull Request

### Code Style

- Use ES6+ features
- Follow [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)
- Maintain inline documentation
- Test across browsers

## 📞 Support

### Getting Help

- 📧 Email: growth-team@rise8.us
- 💬 Slack: #growth-tools channel
- 📚 [Documentation Wiki](#)
- 🐛 [Issue Tracker](https://github.com/cspakes-rise8/rise8-checklist/issues)

### Reporting Issues

Please include:
- Browser version
- Steps to reproduce
- Expected behavior
- Screenshots (if applicable)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Rise8 Growth Team for requirements and testing
- Federal contracting community for feedback
- Open source contributors

---

<div align="center">
  <p>Built with ❤️ by Rise8</p>
  <p>
    <a href="https://rise8.us">Website</a> •
    <a href="https://github.com/rise8">GitHub</a> •
    <a href="https://linkedin.com/company/rise8">LinkedIn</a>
  </p>
</div>
