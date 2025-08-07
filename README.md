# AI Agents Collection for Claude Code

A comprehensive collection of specialized AI agents designed to work with Claude Code, providing expert assistance across engineering, design, marketing, security, testing, and project management domains. Each agent is optimized for specific tasks and can be used as sub-agents within Claude Code's agent system.

> **Inspired by [BMAD-METHOD](https://github.com/bmadcode/BMAD-METHOD)** - This agent collection draws inspiration from the Breakthrough Method for Agile AI-Driven Development (BMAD), which pioneered the concept of specialized AI agents collaborating in rapid development cycles. BMAD's innovative approach to agentic planning and context-engineered development has influenced the design philosophy and rapid development focus of these agents.

## 📥 Installation

### Prerequisites: Install Claude Code

First, install Claude Code if you haven't already:

```bash
# Install Claude Code
curl -fsSL https://claude-code.anthropic.com/install.sh | sh

# Or using npm
npm install -g @anthropic/claude-code
```

### Download and Install Agents

Download this repository:

```bash
git clone https://github.com/marciobarroso/agents.git
```

Copy to your Claude Code agents directory:

```bash
cp -r agents/* ~/.claude/agents/
```

Or manually copy all the agent files to your `~/.claude/agents/` directory.

Restart Claude Code to load the new agents.

## 🚀 Quick Start

Agents are automatically available in Claude Code. Simply describe your task and the appropriate agent will be triggered. You can also explicitly request an agent by mentioning their name.

📚 **Learn more**: [Claude Code Sub-Agents Documentation](https://docs.anthropic.com/claude/docs/claude-code-sub-agents)

### Example Usage

- "Create a new app for tracking meditation habits" → **rapid-prototyper**
- "What's trending on TikTok that we could build?" → **trend-researcher**
- "Our app reviews are dropping, what's wrong?" → **feedback-synthesizer**
- "Make this loading screen more fun" → **whimsy-injector**

## 📋 Overview

This project defines 40+ specialized agents that can be integrated with Claude Code to provide expert-level assistance in various domains. Each agent is designed with specific expertise, tools, and responsibilities to handle different aspects of software development and business operations within rapid development cycles (typically 6-day sprints). The collection includes 2 bonus agents for team morale and performance coaching.

## 📁 Project Structure

```
agents/
   README.md
   bonus/                    # Fun and creative agents
   design/                   # UI/UX and creative design agents  
   engineering/              # Development and technical agents
   marketing/                # Content and growth marketing agents
   product/                  # Product management and research agents
   project-management/       # Launch and project coordination agents
   security/                 # Cybersecurity and compliance agents
   operations/               # Business operations and infrastructure agents
   testing/                  # Quality assurance and performance agents
```

## 🎯 Agent Categories

### Engineering (7 agents)
- **ai-engineer** - AI/ML implementation, LLM integration, computer vision
- **backend-architect** - Server architecture, databases, APIs, scalability
- **devops-automator** - CI/CD, infrastructure, deployment automation
- **frontend-developer** - React, Next.js, modern web development
- **mobile-app-builder** - iOS/Android development, cross-platform solutions
- **rapid-prototyper** - Quick MVP development, proof-of-concept building
- **test-writer-fixer** - Test automation, debugging, code quality

### Design (5 agents)
- **brand-guardian** - Brand consistency, visual identity, guidelines
- **ui-designer** - Interface design, component systems, user experience
- **ux-researcher** - User research, usability testing, design validation
- **visual-storyteller** - Visual content, infographics, presentation design
- **whimsy-injector** - Creative elements, animations, delightful interactions

### Security (6 agents)
- **compliance-auditor** - Regulatory compliance, audit preparation
- **incident-responder** - Security incident handling, forensics
- **penetration-tester** - Vulnerability assessment, security testing
- **security-architect** - Security design, threat modeling, risk assessment
- **security-code-reviewer** - Secure code analysis, vulnerability detection
- **threat-hunter** - Proactive threat detection, security monitoring

### Marketing (7 agents)
- **app-store-optimizer** - ASO, app store presence, download optimization
- **content-creator** - Blog posts, video scripts, cross-platform content
- **growth-hacker** - Growth experiments, viral mechanics, user acquisition
- **instagram-curator** - Instagram strategy, visual content, engagement
- **reddit-community-builder** - Reddit marketing, community engagement
- **tiktok-strategist** - TikTok content, viral trends, short-form video
- **twitter-engager** - Twitter strategy, engagement, thought leadership

### Testing (5 agents)
- **api-tester** - API testing, performance testing, load testing
- **performance-benchmarker** - Performance optimization, benchmarking
- **test-results-analyzer** - Test analysis, quality metrics, reporting
- **tool-evaluator** - Tool assessment, technology evaluation
- **workflow-optimizer** - Process improvement, efficiency optimization

### Project Management (3 agents)
- **experiment-tracker** - A/B testing, experiment design, results analysis
- **project-shipper** - Launch coordination, release management, go-to-market
- **company-producer** - Team coordination, resource management, sprint planning

### Product (3 agents)
- **feedback-synthesizer** - User feedback analysis, insights synthesis
- **sprint-prioritizer** - Feature prioritization, backlog management
- **trend-researcher** - Market research, trend analysis, competitive intelligence

### Operations (5 agents)
- **analytics-reporter** - Data analysis, metrics reporting, insights
- **finance-tracker** - Budget management, financial tracking, cost optimization
- **infrastructure-maintainer** - System maintenance, monitoring, reliability
- **legal-compliance-checker** - Legal review, compliance verification
- **support-responder** - Customer support, issue resolution, documentation

### Bonus (2 agents)
- **joker** - Humor injection, team morale, light-hearted content
- **coach** - Elite performance coaching, agent coordination, motivational leadership

## 🔧 Agent Configuration Format

Each agent follows a standardized YAML frontmatter format:

```yaml
---
name: agent-name
description: Detailed description with usage examples
color: visual-identifier-color
tools: [Write, Read, MultiEdit, Bash, etc.]
---
```

### Key Features:
- **Contextual Examples** - Each agent includes practical usage scenarios
- **Tool Integration** - Specified tools available to each agent
- **Color Coding** - Visual identification for different agent types
- **Sprint Integration** - Optimized for 6-day development cycles
- **Proactive Triggers** - Some agents auto-activate based on context

## 🔗 Integration with Claude Code

These agents are designed to work seamlessly with Claude Code's agent system:

1. **Task Tool Integration** - Agents can be launched using Claude Code's Task tool
2. **Specialized Expertise** - Each agent provides domain-specific knowledge and capabilities  
3. **Tool Access** - Agents have access to appropriate tools for their domain
4. **Context Awareness** - Agents understand rapid development cycles and constraints

### Example Usage:
```
user: "We need to optimize our API performance"
assistant: "I'll use the api-tester agent to analyze your API performance and identify bottlenecks."
```

## 📊 Agent Capabilities

### Common Tools Available:
- **Write/Read/Edit** - File manipulation and content creation
- **Bash** - Command execution and system operations  
- **Grep/Glob** - Code search and file pattern matching
- **WebFetch/WebSearch** - Internet research and data gathering
- **TodoWrite** - Task management and progress tracking

### Specialized Features:
- **Performance Benchmarking** - API response time < 200ms targets
- **Security Standards** - OWASP compliance, threat modeling
- **Design Systems** - Component libraries, accessibility standards
- **Growth Metrics** - Viral coefficients, user acquisition costs
- **Quality Gates** - Automated testing, code coverage requirements

## 💡 Design Philosophy

### Rapid Development Focus
- Optimized for 6-day sprint cycles (inspired by BMAD-METHOD's rapid development approach)
- Balance between speed and quality
- Practical implementation over perfect solutions
- Progressive enhancement approach

### Cross-Functional Collaboration  
- Agents designed to work together (following BMAD's agentic planning principles)
- Consistent communication patterns
- Shared vocabulary and standards
- Integrated workflows

### Business Impact Orientation
- User-centric decision making
- Growth and engagement focused
- Data-driven recommendations
- Revenue and retention optimization

### BMAD-METHOD Influence
- **Agentic Planning**: Specialized agents with deep domain expertise
- **Context-Engineered Development**: Rich context and implementation details in agent specifications
- **Rapid Iteration**: Focus on quick implementation and continuous improvement
- **Human-AI Collaboration**: Agents designed to augment human capabilities rather than replace them

## 📈 Success Metrics

Each agent category has specific KPIs:
- **Engineering**: Build time < 5min, test coverage > 80%
- **Design**: Accessibility score > 95%, load time < 3s
- **Security**: Zero critical vulnerabilities, 99.9% uptime
- **Marketing**: Engagement rate > 5%, conversion rate optimization
- **Testing**: Bug detection rate, performance benchmarks

## 🚀 Getting Started

1. **Browse Agent Categories** - Explore the relevant domain folders
2. **Review Agent Descriptions** - Understand each agent's expertise and examples
3. **Integrate with Claude Code** - Use the Task tool to launch specialized agents
4. **Monitor Performance** - Track agent effectiveness and iterate

## 🤝 Contributing

When adding new agents:
- Follow the established YAML frontmatter format
- Include practical usage examples
- Specify appropriate tools and capabilities
- Consider integration with existing agents
- Optimize for rapid development cycles

## 📄 License

This project is designed for use with Claude Code and follows Anthropic's usage guidelines for AI agent development.

## 🙏 Acknowledgments

This project is inspired by and builds upon the innovative work of the [BMAD-METHOD](https://github.com/bmadcode/BMAD-METHOD) framework, which pioneered the concept of specialized AI agents collaborating in rapid development cycles. The BMAD-METHOD's approach to agentic planning and context-engineered development has significantly influenced the design and philosophy of this agent collection.

---

*Built for rapid innovation and intelligent automation - transforming how teams ship software and grow products.*