# 🚀 Jentic Summer Hackathon 2025

<div align="center">
  <p align="center">
    <a href="https://x.com/JenticAI">
      <img src="https://img.shields.io/badge/Follow%20on%20X-000000?style=for-the-badge&logo=x&logoColor=white" />
    </a>
    <a href="https://www.linkedin.com/company/jentic">
      <img src="https://img.shields.io/badge/Follow%20on%20LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
    </a>
    <a href="https://discord.gg/TdbWXZsUSm">
      <img src="https://img.shields.io/badge/Join%20our%20Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" />
    </a>
  </p>
</div>

Welcome to the Jentic Summer Hackathon! Join us in building the future of AI agents and workflow automation. Whether you have 2 hours or a full weekend, there's a place for you to contribute meaningfully to our open-source ecosystem.

## 🎯 What We're Building

Jentic is building the infrastructure for AI agents to work with real-world APIs and workflows. Our hackathon focuses on expanding this ecosystem through:

- **Standard Agent Framework**: Easy-to-deploy AI agents that work out of the box
- **Arazzo Engine**: Workflow execution engine that connects APIs seamlessly  
- **API Directory**: Comprehensive collection of working API specifications
- **Integration Tools**: Bridges between different AI frameworks and real-world systems

## 🏆 Participation Tiers

Choose your adventure based on your available time and technical comfort level:

### 🌱 Tier 1: Entry Level (2 hours - 1 afternoon)
*Perfect for beginners or quick contributions*

#### Standard Agent Prompt Creation
Create and verify working prompts for our standard agents.

**Example**: "Go grab articles from New York Times about Trump and put on Discord"

**Process**:
1. Propose a prompt idea
2. Test it thoroughly to ensure it works
3. Open a ticket with verification proof
4. Submit to our prompt library

**Reward**: 1 point per verified prompt  
**Dependencies**: Uses standard agent framework and Jentic SDK

---

### 🔧 Tier 2: API Development (Few hours - Full weekend)
*Multiple approaches, minimal stack dependency*

#### Option A: HAR File to OpenAPI Conversion
Transform undocumented APIs into usable specifications.

**Target**: Websites without published APIs (e.g., property sites, restaurant platforms)

**Process**:
1. Identify target websites with hidden APIs
2. Use browser network tab to capture API calls
3. Download HAR (HTTP Archive) files
4. Convert to OpenAPI specifications using your preferred method:
   - Manual transcription
   - Custom utility scripts
   - LLM assistance (Gemini, ChatGPT, etc.)
   - Hybrid approaches

**Deliverable**: PR to our public-apis repository  
**Dependencies**: MINIMAL - only for final submission

#### Option B: Generic API Discovery (Open-Ended)
*"There are websites that don't have APIs or documented APIs. We would like to have their APIs. You figure it out."*

**Methods**: Web scraping, reverse engineering, manual documentation, custom tooling  
**Flexibility**: Choose your own approach  
**Dependencies**: NONE until final submission

#### Option C: Chrome Extension Development
Build a browser extension for automatic API discovery.

**Functionality**:
- Click button on any website
- Auto-generate OpenAPI specification
- Push to Jentic API directory

**Inspiration**: Similar to Notion's web clipper  
**Dependencies**: LOW - extension works independently

---

### ⚡ Tier 3: Advanced Technical (Weekend projects)
*Higher complexity, variable integration levels*

#### OpenAPI Specification Optimization
**Problem**: Current system loads 60,000+ line specs when only needing ~400 lines  
**Solution**: Build tool to extract minimal required specifications  
**Example**: Extract only "create task" functionality from 10,000-line Jira spec  
**Dependencies**: MODERATE - optimizes Arazzo Engine

#### Agent Communication Integrations
**Goal**: Enable standard agent communication through multiple platforms  
**Platforms**: Slack, Discord, Twilio (SMS), Email, Telegram, etc.  
**Dependencies**: HIGH - requires standard agent and system integration

#### LLM-Powered API Discovery System
**Concept**: Use LLMs with web search to automatically find/create OpenAPI specs  
**Challenge**: Hallucination risk management  
**Dependencies**: LOW - can work as standalone tool

#### GraphQL Support in Arazzo Runner
**Minimum**: Implement via graphql-to-openapi conversion  
**Advanced**: Explore native support using Arazzo extensions and integrated GraphQL client  
**Dependencies**: MODERATE - extends Arazzo Engine capabilities

#### API Agent-Readiness Scorecard & Evaluation
**Goal**: Automated assessment of API quality for agent usage  
**Scope**: Check completeness of descriptions, error codes, authentication info, formatting, consistency  
**Advanced**: Score for presence of multi-level API architecture  
**Dependencies**: LOW - standalone evaluation tool

---

### 🧠 Tier 4: Advanced AI Features (Full weekend+)
*Cutting-edge AI research and implementation*

#### New Reasoning Models in Standard Agent
**Goal**: Implement advanced reasoning patterns  
**Models**: LATS, Plan-Act, ReAct, Tree-of-Thoughts  
**Dependencies**: HIGH - deep standard agent framework knowledge

#### Local MCP Support in Standard Agent
**Scope**: Filesystem, Playwright/Puppeteer, local APIs  
**Benefit**: Enable agents to work with local development environments  
**Dependencies**: HIGH - requires standard agent framework

#### Agent Behavior Modification System
**Concept**: Real-time agent reconfiguration through natural language  
**Examples**: "Only run on weekdays", "Never respond to this person"  
**Status**: Not available in initial standard agent version  
**Dependencies**: HIGH - requires deep framework knowledge

#### Doc-to-Arazzo Converter
**Goal**: AI-based process to read official HTML/PDF API documentation and convert to Arazzo workflows  
**Benefit**: Automatically generate executable workflows from human documentation  
**Dependencies**: MODERATE - works with Arazzo format

#### JITT vs Front-loading Evaluation
**Research**: Comparative evaluation of tool calling accuracy  
**Scope**: Front-loaded tools vs just-in-time loading from RAG systems  
**Methodology**: Measure results as number of tools varies, potentially using τ-bench  
**Dependencies**: LOW - standalone research project

#### Prompt Injection Detection
**Goal**: Real-time sanitization system for API responses  
**Focus**: Performance and cost optimization  
**Approach**: Traditional NLP techniques triaging to small language models and LLMs  
**Dependencies**: NONE - standalone security tool

#### Jentic CLI Agent
**Concept**: CLI agent that runs like Claude, Gemini, or Qwen CLI  
**Requirements**: Filesystem tools at minimum  
**Inspiration**: Bring conversational AI to the command line  
**Dependencies**: MODERATE - builds on standard agent

---

### 🛠️ Independent/Standalone Options
*No Jentic stack dependency required*

#### Validation & Quality Assurance Tools
**Purpose**: Verify OpenAPI specifications are compliant and functional  
**Challenge**: Distinguish valid specs from nonsense  
**Dependencies**: NONE - standalone utilities

#### Integration Framework Development
**Goal**: Bridge between Arazzo engine and other agent frameworks  
**Purpose**: Add functionality beyond pure engine capabilities  
**Dependencies**: LOW - designed for external frameworks

## 🎁 Rewards & Recognition

### Point-Based System
- **1 Point**: Simple prompt creation, basic API submission
- **3 Points**: Chrome extension, quality assurance tools
- **5 Points**: Advanced integrations, reasoning model implementation
- **10 Points**: Novel research contributions, complex system implementations

### Prizes
- **Digital**: 3-month subscriptions to AI coding tools (Cursor, GitHub Copilot, etc.)
- **Experience**: Office tours, coffee with founders, mentorship opportunities
- **Recognition**: Featured contributions, community spotlight

## 🚀 Getting Started

### Prerequisites
- **Minimum**: Git, basic programming knowledge
- **Recommended**: Python, API experience
- **Advanced**: AI/ML frameworks, agent development experience

### Quick Start
1. **Fork this repository**
2. **Choose your tier and project**
3. **Join our Discord** for real-time support: [Jentic Community Discord](https://discord.gg/TdbWXZsUSm)
4. **Review project guidelines** in `/docs/contributing.md`
5. **Start building!**

### Development Setup
```bash
# Clone your fork
git clone https://github.com/yourusername/jentic-hackathon.git
cd jentic-hackathon

# Install dependencies (varies by project)
pip install -r requirements.txt  # For Python projects
npm install                      # For JavaScript projects

# Run tests
python -m pytest                # Python
npm test                        # JavaScript
```

## 📋 Submission Guidelines

### For All Tiers
1. **Create a branch** for your contribution
2. **Document your work** with clear README files
3. **Include tests** where applicable
4. **Submit a PR** with detailed description
5. **Open a ticket** describing your contribution

### Quality Standards
- **Working code**: All submissions must be functional
- **Documentation**: Clear setup and usage instructions
- **Testing**: Include basic tests for complex features
- **API specs**: Must be valid OpenAPI 3.0+ format

## 🤝 Support & Community

### Real-Time Help
- **Discord**: `#summer-hackathon` channel for immediate support

### Resources
- **API Directory**: `/apis/` folder with existing specifications
- **Examples**: `/examples/` folder with working samples
- **Docs**: `/docs/` folder with detailed guides
- **Templates**: `/templates/` folder with project starters

## 📅 Event Schedule

### Event Day
- **10:00**: Opening ceremony and project selection
- **12:00**: Hacking begins
- **13:00**: Lunch and networking
- **14:00**: Midday check-in and troubleshooting
- **17:00**: Submission deadline
- **18:00**: Presentations and judging
- **18:30**: Awards and closing


## 📞 Contact & Questions

- **Event Lead**: Rod Rivera (@rodjentic in Discord)
- **General Questions**: `#general` in Discord
- **Technical Issues**: `#summer-hackathon` in Discord

## 🎉 Let's Build the Future Together!

Whether you're contributing a simple prompt or building the next breakthrough in AI agent reasoning, every contribution matters. Join us in making AI agents more capable, reliable, and accessible to everyone.

**Ready to start? Pick your project above and let's build something amazing! 🚀**

---

*This hackathon is part of Jentic's commitment to open-source development and community-driven innovation. All contributions will be recognized and credited appropriately.*
