# Narrative — Career Intelligence Platform

An AI-powered CV optimization platform that uses Google Gemini to analyze job fit, suggest strategic rewrites, provide LinkedIn optimization, and interview coaching. Works for any professional role.

## Quick Start

1. Upload your CV (PDF/DOCX/TXT)
2. 2. Paste the job description
   3. 3. Get instant analysis with your match score, strategic narrative, and recommendations
      4. 4. Optimize your LinkedIn profile
         5. 5. Prepare for the interview with STAR-method coaching
           
            6. ## Features
           
            7. - **CV Calibration**: Smart role detection, match scoring (0-100), professional rewrites
               - - **ATS Optimization**: 92%+ readiness score to pass automated screening
                 - - **LinkedIn Optimization**: Headline, about section, keywords, and profile gaps
                   - - **Interview Prep**: STAR-method questions, sample answers, mock interview practice
                     - - **AI Career Coach**: Real-time feedback and role-specific guidance
                      
                       - ## Tech Stack
                      
                       - - Next.js 14, React 18, TypeScript, Tailwind CSS
                         - - Google Gemini 2.0 Flash AI engine
                           - - Vercel deployment
                            
                             - ## Installation
                            
                             - ```bash
                               git clone https://github.com/fluraz/narrative-ai.git
                               cd narrative-ai
                               npm install
                               cp .env.example .env.local
                               # Add your GOOGLE_API_KEY to .env.local
                               npm run dev
                               ```

                               Open http://localhost:3000

                               ## Environment Variables

                               Create `.env.local`:
                               ```
                               GOOGLE_API_KEY=your_gemini_api_key
                               GEMINI_MODEL=gemini-2.0-flash-exp
                               ```

                               Get a free Gemini API key: https://ai.google.dev

                               ## Deployment

                               Deploy to Vercel (recommended):
                               1. Push code to GitHub
                               2. 2. Connect GitHub to Vercel at vercel.com
                                  3. 3. Add GOOGLE_API_KEY environment variable
                                     4. 4. Deploy
                                       
                                        5. Your app will be live instantly with auto-updates.
                                       
                                        6. ## Security
                                       
                                        7. - No permanent data storage (session-only)
                                           - - Rate limited: 5 analyses per 15 minutes
                                             - - Input sanitization prevents attacks
                                               - - GDPR compliant
                                                
                                                 - ## License
                                                
                                                 - MIT
                                                
                                                 - ---

                                                 Made by fluraz | Live: [narrative-ai.vercel.app](https://narrative-ai.vercel.app)
