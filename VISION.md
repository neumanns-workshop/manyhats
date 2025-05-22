# Many Hats 🎩
*A Personal AI Workshop for ADHD-Optimized Productivity*

## Overview

Many Hats is a comprehensive personal AI ecosystem built around Discord, designed to manage the complexity of modern digital life through specialized AI agents coordinated by a central "Manager Bot." Named after the concept of wearing many hats in different roles, this system provides executive function support particularly valuable for ADHD management.

## Architecture Philosophy

**The Workshop Metaphor**: Neumann's Workshop serves as a digital makerspace where each AI bot acts as a specialized tool, with Many Hats (the Manager Bot) serving as the workshop foreman coordinating all activities.

### Core Components

- **Manager Bot (Many Hats)** - Central orchestrator and strategic intelligence
- **Email Bot** - Email triage, drafting, and management
- **Project Bots** - Dynamic, project-specific intelligence agents
- **Additional Specialized Bots** (planned):
  - Calendar Bot - Scheduling and time management
  - Finance Bot - Expense tracking and financial management
  - Learning Bot - Skill development and course tracking
  - Health Bot - Wellness and medical appointment management

## Current Discord Channels

- `#general` - Many Hats coordination and high-level updates
- `#email` - Email Bot operations with thread-per-email management  
- `#projects` - Project tracking and coordination hub
- `#project-*` - Dynamic project-specific channels with dedicated Project Bots
- `#notes` - Knowledge capture and documentation
- `#bot-admin` - Bot management and configuration
- `#assets` - Shared resources (resumes, templates, etc.)

## Project Bot System

### Dynamic Project Channels
Many Hats automatically creates dedicated channels and specialized bots for significant projects:

**Example Project Channels:**
- `#project-netflix-integration` - Client project with Netflix-specific bot
- `#project-react-mastery` - Learning project with curriculum tracking  
- `#project-job-search-2025` - Job hunting coordination with application tracking

### Project Bot Specialization
Each Project Bot becomes an expert in its domain:
- **Context Awareness** - Understands project goals, tech stack, and constraints
- **Resource Management** - Tracks time, budget, and deliverables
- **Communication** - Manages client/stakeholder interactions
- **Integration** - Connects to relevant emails, calendar events, and GitHub repos
- **Progress Tracking** - Milestone management and deadline monitoring

## Email Bot Features (Phase 1)

### Core Functionality
- **IMAP/SMTP Integration** with Bluehost OX email (`jared@neumannsworkshop.com`)
- **Thread-Based Email Management** - Each important email gets its own Discord thread
- **Document-Aware Responses** - Drafts responses using indexed personal documents
- **Priority Classification** - Automatically categorizes and prioritizes incoming mail

### Email Configuration
```
IMAP: imap.oxcs.bluehost.com:993 (SSL)
SMTP: smtp.oxcs.bluehost.com:587 (STARTTLS)
```

### Planned Email Workflows
1. **Morning Triage**: Automatic email summarization and priority ranking
2. **Smart Drafting**: Context-aware response generation using personal documents
3. **Approval Workflow**: Discord-based review and approval before sending
4. **Follow-up Tracking**: Automatic reminders for pending responses

## Technical Stack

### Current Implementation
- **Python** - Primary development language
- **Discord.py** - Discord bot framework
- **Ollama** - Local LLM integration (Llama 3.1 8B recommended)
- **IMAP/SMTP** - Email protocol handling
- **Vector Database** - Document indexing (ChromaDB/FAISS)

### ADHD-Optimized Features
- **Reaction-Based Quick Actions** - ✅❌📅🔄 for rapid decision making
- **Visual Progress Tracking** - Progress bars and achievement notifications
- **Context Preservation** - Never lose track of where you left off
- **Gentle Accountability** - Supportive reminders and progress celebrations
- **Executive Function Scaffolding** - Break complex tasks into manageable steps

## Installation & Setup

### Prerequisites
- Python 3.8+
- Discord Developer Account
- Ollama installed locally
- Bluehost email credentials

### Environment Setup
```bash
# Clone repository (when available)
git clone https://github.com/neumannsworkshop/many-hats
cd many-hats

# Install dependencies
pip install -r requirements.txt

# Configure environment variables
cp .env.example .env
# Edit .env with your Discord tokens and email credentials

# Start Ollama
ollama serve
ollama pull llama3.1:8b

# Run the Email Bot
python email_bot.py
```

## Development Roadmap

### Phase 1: Email Foundation ✨ *Current Focus*
- [x] Email server integration
- [ ] Basic Discord bot framework
- [ ] Thread-per-email system
- [ ] Document indexing for response generation
- [ ] Simple approval workflow

### Phase 2: Manager Bot & Project System
- [ ] Cross-bot coordination framework
- [ ] Dynamic project channel creation
- [ ] Project-specific bot deployment
- [ ] Priority queue management across projects
- [ ] Strategic analysis and reporting
- [ ] Resource conflict detection and resolution

### Phase 3: Voice Integration
- [ ] Speech-to-text integration (Whisper)
- [ ] Natural language command processing
- [ ] Voice-activated Many Hats interactions
- [ ] Hands-free email management

### Phase 4: Advanced Automation
- [ ] Proactive scheduling and planning
- [ ] Pattern learning from user behavior
- [ ] Autonomous low-priority task handling
- [ ] Cross-domain intelligence insights

## Contributing

This is currently a personal project, but the architecture and patterns developed here may be open-sourced as reusable components for other personal AI systems.

## Philosophy

Many Hats embodies the principle that AI should amplify human capability rather than replace human judgment. Every action requires human approval, but the system handles the cognitive overhead of information processing, context switching, and task coordination.

The goal is to create a digital chief of staff that understands your priorities, maintains context across all your activities, and helps you stay focused on what matters most.

---

*Built in Neumann's Workshop - where AI meets craftsmanship* 🔧

## Contact

- **Website**: [neumannsworkshop.com](https://neumannsworkshop.com)
- **Discord**: Neumann's Workshop
- **Email**: jared@neumannsworkshop.com