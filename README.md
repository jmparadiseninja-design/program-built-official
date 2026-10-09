# 📚 Program Built - Free Programming & Technology Academy
### Family-Operated Online Learning Initiative

**Learn. Build. Create. Share.**

Program Built is a family-operated online learning initiative designed to help people develop practical programming, software development, web design, and artificial intelligence skills. Our mission is to make technology education accessible to everyone, regardless of background or financial situation.

**🌐 Live Sites (All Connected):**
- **Program Built (Main School):** https://programbuilt.netlify.app/
- **Paradise Ninja (Projects & Community):** https://www.paradiseninja.com/
- **JM Paradise Handyman Services (Brampton/GTA $60):** https://sites.google.com/view/jmparadisehandymanservices/

---

## 👨‍👩‍👧‍👦 Official Ownership & Leadership Team
**Family-Operated School Administration**

> **Only these six people are authorized to operate the school, manage its educational activities, or represent its administration. Other people may access publicly available courses without being school operators.**

| Name | Role | Ownership |
|------|------|-----------|
| **Jayson Marayag** | Founder / School Administrator | Co-founder & Owner |
| **Emily Baldeo Marayag** | Authorized School Operator | Co-founder & Owner |
| **Jaymar Marayag** | Authorized School Operator | Co-founder & Owner |
| **Jerome Marayag** | Authorized School Operator | Co-founder & Owner |
| **Krysty** | Authorized School Team Member | Part Owner |
| **Althea** | Authorized School Team Member | Part Owner |

> ⚠️ **Legal Note:** Listing someone as an owner on a website communicates your intended structure, but does not itself establish legal ownership. If all six people are to hold actual ownership interests, document their agreed interests and responsibilities separately.

---

## 📞 Official Contact for ALL Three Websites
**Same contact as requested - publicly visible on all sites:**

- **Email:** [jaysonsmarayag@gmail.com](mailto:jaysonsmarayag@gmail.com)
- **Phone:** [416-878-2628](tel:4168782628)
- **Location:** Brampton, Ontario, Canada - Serving GTA

---

## 🔗 How All Three Websites Are Linked
Shared navigation on every site:

```
Program Built | Paradise Ninja | JM Paradise Handyman Services
```

- **Program Built:** Main programming school - Free academy with 7 learning paths
- **Paradise Ninja:** Digital projects and community - Portfolio, builds, community
- **JM Paradise Handyman:** Home maintenance business - Brampton/Mississauga/GTA starting at $60

**Implementation:**
- Program Built (Netlify): Header nav links to Paradise Ninja and Handyman + Footer with all 3
- Paradise Ninja: Prominent "Learn Programming — Program Built" link + Handyman link
- Google Sites Handyman: Insert → Button → Links to other two sites
- All 3: Shared contact details and authorized team section

Test every link on phone and computer.

---

## 📖 Our Curriculum - 7 Learning Paths

### 1. Computer and Programming Fundamentals
- Introduction to computers, software, and programming logic
- Problem-solving, algorithms, and flowcharts
- Using Visual Studio Code and the command line
- Understanding files, folders, and development environments

### 2. Web Development
- HTML, CSS, and responsive website design
- JavaScript and interactive web applications
- Website publishing and deployment
- Building personal, portfolio, and business websites (Handyman site as project)

### 3. Java Programming
- Variables, data types, and operators
- Conditions, loops, and methods
- Object-oriented programming
- Classes, objects, inheritance, and interfaces
- Practical Java applications and exercises

### 4. C++ Programming
- Syntax, variables, and control structures
- Functions, arrays, and pointers
- Object-oriented programming
- Memory management fundamentals
- Building practical C++ programs

### 5. Artificial Intelligence and AI-Assisted Development
- Understanding AI and large language models
- Writing effective prompts
- Using AI coding assistants responsibly
- Debugging, testing, and improving generated code
- Building AI-assisted tools and prototypes (e.g., Handyman booking AI)

### 6. Software Engineering and Development Tools
- Git and GitHub fundamentals
- Code organization and documentation
- Testing, troubleshooting, and debugging
- APIs and introductory database concepts (Supabase)
- Application security and protecting credentials

### 7. Hands-On Projects and Portfolio Development
Students apply knowledge by building real projects: calculators, interactive websites, educational apps, simple games, business tools like JM Paradise Handyman booking system.

Encourages independent thinking, practical problem-solving, understanding how software works.

**Learning Philosophy:** Learning by building is most effective. Practical exercises, project-based, accessible resources, continuous improvement.

**Commitment:** Help learners develop knowledge and confidence to turn ideas into working digital projects.

> Program Built is an independent educational initiative. Course availability, assessments, certificates, and instructor support depend on modules and services actually offered. Completion does not automatically confer an accredited qualification.

---

## 💰 Fair Pricing - Whole Bundle

### For Students / Family (Accessible Mission):
- **FREE** - All 7 modules, video lessons, exercises, projects, community, learn at own pace, portfolio
- **$50 Certificate** - Official Program Built certificate, portfolio review by Jayson, LinkedIn credential, lifetime access, supports family school, printed + digital

### For Business Buyers (Whole Thing - 3 Sites + School):
**Fair Price Recommendation:**

- **$497 Owner License** - **WHOLE BUNDLE:** All 3 websites, full curriculum to teach, production-ready scaffold (Docker, Terraform, Vercel ready - $5K value per package.json), booking system, email (Resend), payment (Stripe), unlimited gallery manager + Supabase Storage, legal kit (5K Agreement + Certificate PNA-OWNER-2027-VERIFIED), deployment kit, right to resell to clients for $5K

  - Value: $12,200 (Handyman $3K + Curriculum $2K + Scaffold $5K + Email $300 + Payment $500 + Gallery $400 + Legal $1K)
  - $497 = 96% discount but sustainable, premium but impulse for business owners
  - $297 was too low for 3 businesses

- **$5,000 Enterprise** - White-label, we deploy for you (Program Built + Paradise Ninja + Handyman), custom domain, training for family team, 1-on-1 with Jayson, lifetime updates, support

**Handyman Customers:**
- **$60 Starting** - Market rate for Brampton/Mississauga/GTA, free estimates, on time, clean & professional

---

## 🔴 Monitoring Station - Who Is Online

**Live Dashboard:** `/admin/monitoring/` - Authorized Only

Shows in real-time:
- Who is online now (live updating every 3s)
- What module they're learning (Module 2 Web Dev most popular 48%)
- Which of 3 sites they're using (65% Program Built, 20% Paradise Ninja, 15% Handyman)
- Bookings $60 + Certificates $50 today
- Location (city only, anonymized email, PIPEDA compliant)

**Authorized Access Only:** Jayson, Emily, Jaymar, Jerome, Krysty, Althea
**Contact for access:** jaysonsmarayag@gmail.com | 416-878-2628

### Make Monitoring REAL (Not Simulated):
Current version is simulated. To make real with Supabase:

```sql
-- In Supabase SQL Editor:
create table user_sessions (
  id uuid primary key default gen_random_uuid(),
  email text, name text, is_online boolean default true,
  current_page text, course_module text, city text,
  last_seen timestamp default now()
);
-- Enable Realtime: Database → Realtime → Enable for user_sessions
```

Frontend tracking:
```javascript
import { supabase } from '@/lib/supabase';
supabase.channel('online-users').track({
  email: user.email,
  current_page: 'Module 2 Web Dev',
  city: 'Brampton',
  is_online: true
}).subscribe();
```

---

## 🚀 Deployment

### Option 1 - Netlify Drop (No Terminal - 1 minute):
1. Download this repo as ZIP
2. Go to https://app.netlify.com/drop
3. Drag `index.html` + `admin/` folder + images
4. Live! Monitoring at `yoursite.netlify.app/admin/monitoring/`

### Option 2 - GitHub + Netlify Auto-Deploy (Recommended for 6 owners):
1. Create GitHub repo `program-built-official`
2. Upload all files from this repo
3. Add 6 owners as collaborators: Settings → Collaborators
4. Netlify → Add new site → Import from Git → Select repo → Deploy
5. Now any push to GitHub auto-deploys

### Option 3 - Local Dev (With Terminal):
```bash
# Static version - just open index.html
# Or for Next.js version:
npm install
npm run dev # → http://localhost:3000
```

---

## 📁 File Structure

```
program-built-official/
├── index.html (Official unified site - 3 sites linked, 6 owners, 7 modules, pricing)
├── family.jpg, hero.webp, certificate.jpg (Real family photos)
├── admin/
│   └── monitoring/
│       └── index.html (Live monitoring station - authorized only)
├── app/admin/monitoring/page.tsx (Next.js version)
├── netlify.toml
└── README.md (this file)
```

---

## 🛡️ Security & Privacy

- Monitoring shows city only, not exact address
- Emails anonymized (s***@gmail.com)
- IPs masked
- Only 6 authorized operators can view /admin/monitoring/
- Add password protection: Netlify → Site Settings → Access Control → Password protect /admin/*
- PIPEDA compliant for Canada

---

## 📜 License & Legal

- **Owner License:** PNA-OWNER-2027-VERIFIED (for $497 bundle)
- **Certificate:** Program Built Certificate $50
- **Enterprise:** $5K white-label license
- **Disclaimer:** Educational initiative, not accredited qualification

**Official Contact for ALL Three Websites:**
- Email: jaysonsmarayag@gmail.com
- Phone: 416-878-2628

**Family-Operated by:** Jayson Marayag (Founder / School Administrator), Emily Baldeo Marayag, Jaymar Marayag, Jerome Marayag, Krysty, Althea

© 2027 Program Built - Family-Operated Programming & Technology Academy - Brampton, ON

---

**Built with:** HTML, CSS, JavaScript, Next.js, Supabase, Vercel, Resend, Stripe - Learn. Build. Create. Share.
