# Narrative AI

Strategic career calibration for modern professionals

AI-powered career storytelling platform that helps professionals optimize their CV, LinkedIn profile, and interview preparation across all industries.

![Narrative AI](https://img.shields.io/badge/status-active-success.svg)
![Next.js](https://img.shields.io/badge/Next.js-14-black)
![TypeScript](https://img.shields.io/badge/TypeScript-5-blue)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

---

## ✨ Features

### 🎯 CV Optimizer

- Upload CV (PDF/DOCX/TXT)
- - AI role detection (automatic)
  - - Match scoring (0-100)
    - - Professional rewrite with industry-specific metrics
      - - ATS-optimized export
       
        - ### 💼 LinkedIn Profile Builder
       
        - - Headline optimization (60 chars)
          - - About section storytelling (3 paragraphs)
            - - Top 10 SEO keywords
              - - Experience bullet points
               
                - ### 🎤 Interview Prep
               
                - - STAR-method questions (5-7 per role)
                  - - Sample answers based on your CV
                    - - Behavioral scenarios
                      - - Practice tips
                       
                        - ### 💬 AI Career Coach
                       
                        - - Contextual career advice
                          - - Real-time feedback
                            - - Strategy recommendations
                              - - Progress tracking
                               
                                - ---

                                ## 🎨 Brand Identity

                                **Colors:**

                                - Bone: #F8F8F6 (primary background)
                                - - Gold: #D4B483 (accent)
                                  - - Navy: #4b5563 (text)
                                   
                                    - **Typography:**
                                   
                                    - - Inter Light (300) for headlines
                                      - - Inter Regular (400) for body
                                        - - Never exceed font-weight 500
                                         
                                          - **Design Philosophy:**
                                         
                                          - - Premium but accessible
                                            - - Calm and sophisticated
                                              - - Universal (works for all roles)
                                                - - Evidence-based (no hype)
                                                 
                                                  - ---

                                                  ## 🚀 Quick Start

                                                  ### Prerequisites

                                                  - Node.js 18+
                                                  - - Google Gemini API key ([Get one here](https://aistudio.google.com/app/apikey))
                                                   
                                                    - ### Installation
                                                   
                                                    - ```bash
                                                      # Clone repository
                                                      git clone https://github.com/yourusername/narrative-ai.git
                                                      cd narrative-ai

                                                      # Install dependencies
                                                      npm install

                                                      # Setup environment variables
                                                      cp .env.example .env.local

                                                      # Add your GOOGLE_API_KEY to .env.local

                                                      # Run development server
                                                      npm run dev

                                                      # Open http://localhost:3000
                                                      ```

                                                      ---

                                                      ## 🔐 Environment Variables

                                                      Create .env.local in the root directory:

                                                      ```bash
                                                      # REQUIRED
                                                      GOOGLE_API_KEY=your_gemini_api_key_here
                                                      GEMINI_MODEL=gemini-2.0-flash-exp

                                                      # OPTIONAL (Production)
                                                      REDIS_URL=redis://localhost:6379

                                                      # OPTIONAL (Week 2 - Supabase)
                                                      NEXT_PUBLIC_SUPABASE_URL=https://xxx.supabase.co
                                                      NEXT_PUBLIC_SUPABASE_ANON_KEY=your_anon_key
                                                      SUPABASE_SERVICE_KEY=your_service_key
                                                      ```

                                                      ---

                                                      ## 📁 Project Structure

                                                      ```
                                                      narrative-ai/

                                                      ├─ app/
                                                      │  ├─ page.tsx                    # Main campaign flow
                                                      │  ├─ layout.tsx                  # Root layout
                                                      │  ├─ api/
                                                      │  │  ├─ analyze/route.ts         # CV analysis
                                                      │  │  ├─ chat/route.ts            # AI coach
                                                      │  │  └─ interview-prep/route.ts  # Interview questions
                                                      │  ├─ privacy/page.tsx            # Privacy Policy
                                                      │  └─ terms/page.tsx              # Terms of Service
                                                      │
                                                      ├─ components/
                                                      │  ├─ cv-optimizer/               # CV module components
                                                      │  ├─ linkedin/                   # LinkedIn module
                                                      │  ├─ interview/                  # Interview prep module
                                                      │  ├─ chat/                       # AI coach chat
                                                      │  └─ shared/                     # Shared UI components
                                                      │
                                                      ├─ lib/
                                                      │  ├─ geminiService.ts            # AI analysis engine
                                                      │  ├─ rateLimiter.ts              # Rate limiting
                                                      │  ├─ security.ts                 # Input sanitization
                                                      │  └─ fileParser.ts               # PDF/DOCX parsing
                                                      │
                                                      └─ types/                         # TypeScript definitions
                                                      ```

                                                      ---

                                                      ## 🛡️ Security Features

                                                      - **Rate Limiting:** 5 analyses per 15 minutes, 20 chat messages per hour
                                                      - - **Input Sanitization:** XSS prevention with DOMPurify
                                                        - - **SQL Injection Protection:** Pattern detection and blocking
                                                          - - **Security Headers:** CSP, X-Frame-Options, etc.
                                                            - - **GDPR Compliance:** Cookie consent, Privacy Policy, data rights
                                                             
                                                              - ---

                                                              ## 📊 API Endpoints

                                                              | Endpoint | Method | Rate Limit | Purpose |
                                                              |----------|--------|------------|---------|
                                                              | /api/analyze | POST | 5 per 15 min | CV analysis |
                                                              | /api/chat | POST | 20 per hour | AI coach chat |
                                                              | /api/interview-prep | POST | Same as analyze | STAR questions |
                                                              | /api/export-docx | POST | 10 per day | DOCX generation |

                                                              ---

                                                              ## 🎯 Roadmap

                                                              ### ✅ Week 1: COMPLETE

                                                              - [x] Rate limiting
                                                              - [ ] - [x] Input sanitization
                                                              - [ ] - [x] Security headers
                                                              - [ ] - [x] Cookie consent
                                                              - [ ] - [x] Privacy Policy
                                                              - [ ] - [x] Terms of Service
                                                             
                                                              - [ ] ### 🔄 Week 2: IN PROGRESS
                                                             
                                                              - [ ] - [ ] Supabase authentication
                                                              - [ ] - [ ] Save analyses to database
                                                              - [ ] - [ ] User dashboard
                                                              - [ ] - [ ] GDPR data export
                                                              - [ ] - [ ] Account deletion
                                                             
                                                              - [ ] ### 📅 Week 3: UX Improvements
                                                             
                                                              - [ ] - [ ] Better error handling
                                                              - [ ] - [ ] Progress saving
                                                              - [ ] - [ ] Version history
                                                              - [ ] - [ ] Vercel Analytics
                                                              - [ ] - [ ] Mobile polish
                                                             
                                                              - [ ] ### 📅 Week 4: Monetization
                                                             
                                                              - [ ] - [ ] Stripe integration
                                                              - [ ] - [ ] Free tier (3 analyses/month)
                                                              - [ ] - [ ] Pro tier ($12/month)
                                                              - [ ] - [ ] Subscription management
                                                             
                                                              - [ ] ---
                                                             
                                                              - [ ] ## 🚢 Deployment
                                                             
                                                              - [ ] ### Vercel (Recommended)
                                                             
                                                              - [ ] ```bash
                                                              - [ ] # Install Vercel CLI
                                                              - [ ] npm i -g vercel
                                                             
                                                              - [ ] # Login
                                                              - [ ] vercel login
                                                              - [ ] 
                                                              # Deploy
                                                              vercel

                                                              # Add environment variable
                                                              vercel env add GOOGLE_API_KEY production

                                                              # Deploy to production
                                                              vercel --prod
                                                              ```

                                                              ### Environment Variables in Vercel

                                                              Go to Project Settings → Environment Variables:

                                                              - GOOGLE_API_KEY: Your Gemini API key
                                                              - GEMINI_MODEL: gemini-2.0-flash-exp
                                                              - REDIS_URL (optional): Redis connection string

                                                              ---

                                                              ## 🤝 Contributing

                                                              Contributions are welcome! Please read our [Contributing Guide](CONTRIBUTING.md) first.

                                                              1. Fork the repository
                                                              2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
                                                              3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
                                                              4. Push to the branch (`git push origin feature/AmazingFeature`)
                                                              5. Open a Pull Request

                                                              ---

                                                              ## 📄 License

                                                              This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

                                                              ---

                                                              ## 📞 Contact

                                                              **Project Maintainer:** Emil

                                                              **Email:** [your-email@example.com]

                                                              **Project Link:** [https://github.com/yourusername/narrative-ai](https://github.com/yourusername/narrative-ai)

                                                              ---

                                                              ## 🙏 Acknowledgments

                                                              - [Next.js](https://nextjs.org/) - React framework
                                                              - [Google Gemini](https://ai.google.dev/) - AI analysis
                                                              - [Tailwind CSS](https://tailwindcss.com/) - Styling
                                                              - [Vercel](https://vercel.com/) - Hosting

                                                              ---

                                                              Built with ❤️ for professionals worldwide
