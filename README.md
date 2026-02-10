# AI-Powered Restaurant Assistant

> An intelligent culinary assistant that empowers waitstaff with chef-level knowledge to deliver personalized dining experiences.

## Overview

The AI-Powered Restaurant Assistant is a waiter-facing intelligent system that provides real-time culinary knowledge and recommendations during customer service. It bridges the gap between kitchen expertise and customer experience by enabling waitstaff to answer detailed questions about dishes, suggest personalized recommendations, and accommodate dietary restrictions with confidence.

## Key Features

### Phase 1 - AI Chef Assistant (Current)

- **Intelligent Dish Information**: Answer detailed questions about ingredients, preparation methods, flavor profiles, and allergens
- **Smart Recommendations**: Suggest dishes based on customer preferences, dietary restrictions, and flavor profiles
- **Pairing Suggestions**: Recommend complementary appetizers, sides, and beverages
- **Session Management**: Maintain conversation context for each table throughout the dining experience
- **Allergen Safety**: Comprehensive allergen tracking with cross-contamination warnings
- **Natural Language Interface**: Intuitive query system that understands waiter questions in plain English

### Future Phases

- **Phase 2**: Persistent customer taste profiles across visits
- **Phase 3**: Group intelligence for families, friends, and couples
- **Phase 4**: Cross-restaurant profiles and analytics platform

## Architecture

### Technology Stack

**Frontend**:
- Mobile-responsive web interface
- Offline caching for frequently accessed dishes
- Real-time query processing

**Backend**:
- RESTful API architecture
- Serverless compute (AWS Lambda)
- Natural language processing via LLM integration

**Data Layer**:
- NoSQL database (DynamoDB) for menu and session data
- In-memory caching (Redis) for performance
- Long-term archival storage (S3)

**AI/ML**:
- Amazon Bedrock for LLM capabilities
- Custom recommendation engine
- Intent classification and entity extraction

### AWS Deployment

The system is deployed on AWS using a serverless-first architecture:

- **API Gateway**: RESTful API management
- **Lambda**: Serverless compute for all business logic
- **DynamoDB**: Primary data storage
- **ElastiCache (Redis)**: High-performance caching
- **Bedrock**: LLM integration
- **CloudFront + S3**: Frontend hosting and CDN
- **CloudWatch + X-Ray**: Monitoring and tracing

See [design.md](./design.md#aws-deployment-architecture) for detailed architecture diagrams and configuration.

