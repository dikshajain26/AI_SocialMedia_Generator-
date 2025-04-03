**Project Report: AI-Powered Social Media Content Generator Chatbot**

---

## 1. Introduction
With the rise of digital marketing, social media content has become a key driver for engagement and brand awareness. This project presents an AI-powered chatbot developed using Flowise, designed to generate creative and trending social media content ideas. The chatbot provides real-time, customized content suggestions based on user queries.

## 2. Objectives
- Automate social media content idea generation.
- Ensure relevance by incorporating trending topics.
- Provide diverse content suggestions tailored to various platforms.
- Enhance user engagement through interactive chatbot responses.

## 3. Technology Stack
- **Flowise**: No-code AI workflow tool for chatbot creation.
- **Google Gemini (ChatGoogleGenerativeAI)**: Primary chat model for generating responses.
- **Serper**: API-based search engine to fetch up-to-date industry trends.
- **HTML & JavaScript**: Embedded chatbot integration on websites.

## 4. System Architecture
The chatbot operates using the following agent flow:
- **Supervisor Agent**: Manages the workflow, ensuring responses are structured correctly.
- **Content Idea Generator (Worker Agent)**: Uses the system prompt (as given in the attached image) to craft relevant content ideas.
- **ChatGoogleGenerativeAI (Gemini API)**: Handles conversational responses based on user queries.
- **Serper API**: Provides real-time updates on industry trends and social media discussions.

  ![image](https://github.com/user-attachments/assets/fb67c4e7-f7aa-403d-9bf3-081c1fce18f7)


## 5. Implementation
### 5.1 Chatbot UI Customization
- **Bot Avatar & Icons**: Custom AI bot and user avatars.
- **Welcome Message**: Engaging and user-friendly greeting.
- **Background Theme**: A visually appealing design aligning with social media aesthetics.
- **Starter Prompts**: Predefined suggestions for user interactions.

  ![image](https://github.com/user-attachments/assets/a4aad110-e094-4286-a6da-463fea57c20d)


### 5.2 Code Snippet for Chatbot Integration
The chatbot is embedded using the following HTML and JavaScript:
```html
<flowise-fullchatbot></flowise-fullchatbot>
<script type="module">
    import Chatbot from "https://cdn.jsdelivr.net/npm/flowise-embed/dist/web.js"
    Chatbot.initFull({
        chatflowid: "93264ca2-d67f-4e47-b9c2-64c2cebfcc8d",
        apiHost: "https://flowise.erudites.in",
        theme: {
            button: {
                backgroundColor: '#ff4f64',
                right: 20,
                bottom: 20,
                size: 60,
                dragAndDrop: true,
                iconColor: 'white',
                customIconSrc: 'https://i.imgur.com/GZJ4dAk.png',
                autoWindowOpen: {
                    autoOpen: true,
                    openDelay: 2,
                    autoOpenOnMobile: true
                }
            },
            chatWindow: {
                showTitle: true,
                title: 'Social AI Bot 🤖',
                titleAvatarSrc: 'https://i.imgur.com/RDssvLP.png',
                welcomeMessage: '👋 Hey there! Need help with social media content? Let’s get creative!',
                backgroundColor: '#ffffff',
                backgroundImage: 'https://i.imgur.com/zXpDXPF.jpg',
                fontSize: 16,
                starterPrompts: [
                    "📢 Generate a viral tweet",
                    "📸 Suggest Instagram captions",
                    "📍 Best hashtags for my post",
                    "🎭 Trendy TikTok video ideas"
                ]
            }
        }
    })
</script>
```

## 6. Sample Chat Interaction
### **User Query:** "Create a 1-week content calendar for a bakery's Instagram."
### **Bot Response:**

![image](https://github.com/user-attachments/assets/ff249339-4999-4705-8c7a-fd69edbcde66)

![image](https://github.com/user-attachments/assets/70905661-0b17-4ff4-88d2-62513ba8b9a0)

![image](https://github.com/user-attachments/assets/e1bd6221-fac7-493a-840d-93fc6a0b5c09)

![image](https://github.com/user-attachments/assets/d847d288-db40-4688-b0cb-aaf6c0b23458)


## 7. Future Enhancements
- **Multilingual Support**: Expand the chatbot's capabilities for non-English content creation.
- **Advanced Analytics**: Integrate tracking tools to measure engagement.
- **Personalized AI Recommendations**: Enable AI to analyze past user interactions for refined content suggestions.

## 8. Conclusion
The AI-powered chatbot successfully automates the generation of engaging, niche, and trending social media content. Its integration with Flowise, Google Gemini, and Serper ensures up-to-date and highly relevant content ideas, making it a valuable tool for social media marketers and brands.
