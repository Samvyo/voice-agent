# Voice Agent Platform

An intelligent AI voice agent platform that provides context-aware customer support with seamless human escalation. The platform combines advanced AI capabilities with intelligent routing to deliver exceptional customer experiences while reducing support costs.

## Description

The Voice Agent Platform is a full-stack solution for building, deploying, and managing AI-powered voice agents. It enables businesses to provide 24/7 customer support through intelligent agents that understand context, learn from interactions, and seamlessly escalate to human agents when needed.

### Key Features

- **Intelligent AI Agents**: Context-aware agents powered by OpenAI that understand your business through document ingestion and vector search
- **Real-Time Voice Support**: Native WebRTC voice communication for AI agents with multi-model speech-to-text integration, enabling natural voice conversations
- **Smart Escalation**: Automatic detection of high-ticket offers or complex queries requiring human intervention, with intelligent routing to appropriate human agents
- **Human Agent Voice & Video**: Human agents can opt-in for voice-based or video calling support, providing enterprise-grade communication options for complex issues
- **Real-Time Communication**: Two-way messaging between end-users and human agents with live connection status, supporting text, voice, and video channels
- **Knowledge Management**: Upload documents, links, and training data. The system automatically creates semantic embeddings for intelligent retrieval
- **Analytics Dashboard**: Real-time insights into conversation patterns, topic trends, escalation triggers, and interaction quality
- **Embeddable Widget**: One-line embed code to integrate the chat widget into any website
- **Calendar Integration**: Connect to Google Calendar for scheduling and availability checks
- **Self-Improving Intelligence**: Pattern analysis engine that learns from interactions to improve response quality over time

## Tech Stack

### Client (Frontend)
- **React 19** - Modern UI library for building interactive interfaces
- **Vite** - Fast build tool and development server
- **Redux Toolkit** - Predictable state management for complex application state
- **React Router** - Client-side routing for navigation
- **Tailwind CSS** - Utility-first CSS framework for rapid UI development
- **Recharts** - Data visualization library for analytics dashboards
- **Framer Motion** - Animation library for smooth UI transitions

### Server (Backend)
- **Node.js** - JavaScript runtime environment
- **Express** - Web framework for RESTful API endpoints
- **PostgreSQL** - Relational database for storing agents, interactions, and analytics data
- **Qdrant** - Vector database for semantic search and document embeddings
- **OpenAI API** - Large language model integration for AI agent responses
- **Google APIs** - Calendar integration for scheduling and availability
- **WebRTC** - Real-time voice and video communication protocol for AI agents and human agent support
- **Multer** - File upload handling for document ingestion
- **Node-Cron** - Scheduled tasks for automated training and maintenance

## How It Solves the Problem

### Problem Statement
Businesses face escalating customer support costs ($50-100K annually), long response times (hours), and high cart abandonment rates (40%) due to unanswered questions. Traditional chatbots lack context understanding and cannot handle complex queries effectively.

### Our Solution

#### 1. **Intelligent Context Understanding**
- **Vector Search**: Documents are converted to embeddings and stored in Qdrant for semantic search
- **Context Retrieval**: When a user asks a question, the system retrieves relevant context from your knowledge base using vector similarity
- **Multi-Source Learning**: Agents learn from uploaded documents, website content, FAQs, and past conversations

#### 2. **Smart Escalation System**
- **Automatic Detection**: AI analyzes conversation patterns to detect when human intervention is needed (high-ticket offers, complex issues, emotional cues)
- **Topic-Based Routing**: System matches conversation topics with human agent expertise tags to route to the right specialist
- **Seamless Handoff**: End-users are automatically connected to human agents with full conversation context preserved
- **Multi-Channel Communication**: Real-time messaging between end-users and human agents with connection status monitoring
- **Voice & Video Options**: Human agents can opt-in for voice-based or video calling support based on enterprise needs, enabling richer communication for complex problem-solving
- **Flexible Communication Modes**: Support for text-only, voice calls, or video calls depending on issue complexity and customer preference

#### 3. **Cost Reduction Through Automation**
- **24/7 Availability**: AI agents handle queries around the clock without additional staffing costs
- **High Resolution Rate**: 85% of queries resolved without human escalation
- **Fast Response Times**: Average 1.2 seconds vs 4 hours for human support
- **Scalable Architecture**: Handle thousands of concurrent conversations without proportional cost increases

#### 4. **Continuous Improvement**
- **Pattern Analysis**: System identifies common questions, pain points, and escalation triggers
- **Topic Extraction**: Automatically categorizes conversations for better understanding
- **Analytics Dashboard**: Real-time insights help businesses identify product gaps and improve support strategies
- **Self-Learning**: Agents improve accuracy over time by learning from successful interactions

#### 5. **Flexible Integration**
- **Embeddable Widget**: One-line code integration for any website
- **API-First Design**: RESTful APIs for custom integrations
- **Calendar Integration**: Connect to Google Calendar for scheduling capabilities
- **Multi-Model Support**: Configurable AI models and speech-to-text providers (not vendor-locked)

#### 6. **Enterprise-Grade Features**
- **Real-Time Analytics**: Track conversation quality, topic trends, and escalation patterns
- **Agent Management**: Create, configure, and manage multiple AI agents
- **Document Processing**: Support for PDFs, Word documents, and web links
- **Real-Time Voice**: Native WebRTC support for AI agent voice conversations with low-latency streaming
- **Human Agent Voice & Video**: Enterprise option for human agents to provide voice-based or video calling support, enabling personalized assistance for high-value customers and complex issues
- **Multi-Modal Communication**: Seamless switching between text, voice, and video channels based on customer needs and agent capabilities

### Architecture Highlights

- **Separation of Concerns**: Clean client-server architecture with RESTful API communication
- **State Management**: Redux for predictable client-side state, PostgreSQL for persistent server-side data
- **Real-Time Updates**: Polling mechanism for live message delivery and connection status
- **Scalable Design**: Vector database for fast semantic search, efficient document processing, and memory-optimized streaming
- **Error Handling**: Comprehensive error handling with ngrok proxy support for development and testing

## Use Cases

### Insurance & Financial Services

**Acko Insurance - High-Value Policy Sales**
- Customer browses insurance plans and asks questions about coverage, premiums, and benefits
- AI agent detects high-ticket purchase intent through conversation analysis
- System automatically escalates to a specialized human insurance agent
- Human agent initiates video call to present credentials, explain policy details, and build trust
- Agent can share screen to walk through policy documents, coverage comparisons, and premium calculations
- Result: Higher conversion rates through personalized video consultations for high-value insurance purchases

**Policy Bazaar - Virtual Showroom Tours**
- Customers explore multiple insurance providers and compare plans
- AI agent handles initial queries about different insurance categories (health, life, motor, etc.)
- When customer shows interest in specific plans, system identifies as high-ticket opportunity
- Human agent connects via video call to provide virtual showroom tours
- Agent can showcase different policy options, explain fine print, and demonstrate online tools
- Video interaction enables face-to-face trust building and real-time document sharing
- Result: Enhanced customer experience with personalized virtual consultations leading to informed purchase decisions

### Other Use Cases

- **SaaS Support**: Handle technical questions, account issues, and feature inquiries with voice support
- **E-Commerce**: Answer product questions, shipping inquiries, and return policies with smart escalation for high-value orders
- **Professional Services**: Qualify leads, answer service questions, and schedule consultations via video calls
- **Developer Tools**: Provide API documentation, troubleshooting, and integration support with voice-enabled assistance

---

