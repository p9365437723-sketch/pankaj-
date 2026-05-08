# 🎓 Pankaj Sir Study Hub

A **production-ready educational platform** built with React, Next.js, Firebase, and Tailwind CSS.

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-Production%20Ready-brightgreen)

---

## ✨ Features

✅ **Complete Authentication System**
- Email/Password signup & login
- Google Sign-In integration
- Admin login with secure credentials
- Persistent login sessions
- User blocking system

✅ **Student Portal**
- Class selection (9, 10)
- Subject browsing
- Chapter management
- Rich content viewing
- Interactive quizzes (MCQ)

✅ **Admin Dashboard**
- User management (view, block, delete)
- Content management system
- Chapter CRUD operations
- Real-time user tracking
- Analytics dashboard

✅ **Content System**
- Notes with rich formatting
- Timeline/historical events
- Question banks (1, 3, 5 marks)
- Key terms & definitions
- Important personalities
- Quiz with automatic scoring

✅ **Modern UI/UX**
- Dark green academic theme
- Glassmorphism effects
- 3D floating cards
- Smooth animations
- Mobile responsive design
- Tailwind CSS styling

✅ **Real-time Features**
- Live Firestore updates
- Real-time user tracking
- Instant content synchronization
- No page refreshes needed

✅ **100% FREE**
- No payment system
- All features unlocked for students
- Complete access to all content

---

## 🚀 Quick Start (For Beginners)

### Step 1: Create GitHub Account
1. Go to https://github.com/signup
2. Create free account
3. Verify email

### Step 2: Fork or Clone This Project
1. Go to https://github.com/pankajsir/pankaj-study-hub
2. Click **"Fork"** button (or clone if it's your own)

### Step 3: Create Firebase Project
1. Go to https://firebase.google.com/
2. Click **"Get Started"**
3. Sign in with Google
4. Click **"Create Project"**
   - Name: `pankaj-study-hub`
   - Continue → Continue → Create Project
5. Go to **Project Settings** (gear icon)
   - Copy your Firebase config values

### Step 4: Get Firebase Config Values
In Firebase Console:
1. Go to **Project Settings** → **General**
2. Scroll down to "Your apps"
3. Copy these values:
```
NEXT_PUBLIC_FIREBASE_API_KEY
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN
NEXT_PUBLIC_FIREBASE_PROJECT_ID
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID
NEXT_PUBLIC_FIREBASE_APP_ID
```

### Step 5: Enable Firebase Services

**Enable Authentication:**
1. Go to **Authentication** → **Sign-in method**
2. Click **Email/Password** → Enable → Save
3. Click **Google** → Enable → Configure (add your project)

**Create Firestore Database:**
1. Go to **Firestore Database**
2. Click **Create Database**
3. Select **Start in Test mode**
4. Choose region close to you
5. Click **Create**

### Step 6: Deploy to Vercel (Easy Way!)

1. Go to https://vercel.com/signup
2. Sign up with GitHub
3. Click **"New Project"**
4. Select your GitHub repository
5. Click **"Import"**
6. Under **Environment Variables**, add:
   - `NEXT_PUBLIC_FIREBASE_API_KEY` = your value
   - `NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN` = your value
   - `NEXT_PUBLIC_FIREBASE_PROJECT_ID` = your value
   - `NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET` = your value
   - `NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID` = your value
   - `NEXT_PUBLIC_FIREBASE_APP_ID` = your value
7. Click **"Deploy"**
8. Wait 2-3 minutes...
9. Your site is live! 🎉

---

## 🔐 Default Credentials

### Admin Login
```
ID: p936543773
Password: 9365437723
```

### Student
- Create account on signup page
- Or sign in with Google

---

## 📱 Access Your Site

After Vercel deployment:
- Your site URL: `https://your-project-name.vercel.app`
- Share this URL with students!

---

## 👨‍💻 For Developers

### Local Development

```bash
# Clone repository
git clone https://github.com/yourusername/pankaj-study-hub.git
cd pankaj-study-hub

# Install dependencies
npm install

# Create .env.local file with Firebase values
cp .env.example .env.local
# Edit .env.local and add your Firebase config

# Run development server
npm run dev

# Visit http://localhost:3000
```

### Project Structure

```
pankaj-study-hub/
├── app/
│   ├── layout.js          # App layout
│   ├── globals.css        # Global styles
│   └── page.jsx           # Main app component
├── lib/
│   └── firebase.js        # Firebase config
├── package.json           # Dependencies
├── tailwind.config.js     # Tailwind config
├── next.config.js         # Next.js config
└── README.md              # This file
```

### Key Files

- **app/page.jsx** - Main application (Auth, Student Portal, Admin Dashboard)
- **lib/firebase.js** - Firebase initialization
- **package.json** - All dependencies listed

### Firebase Database Structure

Automatically created when users signup:

```
users/
├── userId
│   ├── name
│   ├── email
│   ├── role (student/admin)
│   ├── isBlocked
│   └── lastLogin

chapters/
├── chapterId
│   ├── title
│   ├── notes
│   ├── quiz
│   ├── keyTerms
│   └── ... (more fields)
```

---

## 🎯 Usage Guide

### For Students

1. **Sign Up**
   - Click "Sign Up"
   - Enter name, email, password
   - Or sign in with Google

2. **Choose Class**
   - Select Class 9 or 10

3. **Choose Subject**
   - Select from: English, Hindi, Science, Social Science

4. **Choose Chapter**
   - Browse available chapters
   - Click to open

5. **Learn**
   - Read notes (📜 tab)
   - View timeline (📅 tab)
   - Check questions (✏️ 📝 📖 tabs)
   - Learn terms (📚 tab)
   - Take quiz (❓ tab)

### For Admin

1. **Login**
   - Click "Admin" tab
   - ID: `p936543773`
   - Password: `9365437723`

2. **Manage Users**
   - View all students
   - Block/unblock students
   - Delete accounts

3. **Add Content**
   - Go to Content tab
   - Select Class → Subject
   - Click "Add New Chapter"
   - Fill in all fields
   - Click "Save Chapter"

4. **Edit Content**
   - Click "Edit" on any chapter
   - Update fields
   - Click "Update Chapter"

5. **Delete Content**
   - Click "Delete" on any chapter
   - Confirm deletion

---

## 📊 Sample Content Format

### Adding a Chapter

**Title:** Chapter 1: The Journey Begins

**Notes:**
```
This chapter introduces students to the concept of...
[Long form educational content here]
```

**1 Mark Questions:**
```
1. What is photosynthesis?
2. Define ecosystem.
3. What is biodiversity?
```

**3 Mark Questions:**
```
1. Explain the water cycle with examples.
2. Describe the layers of atmosphere.
```

**5 Mark Questions:**
```
1. Discuss the impact of deforestation on biodiversity.
```

**Key Terms (JSON):**
```json
{
  "Photosynthesis": "Process by which plants make food using sunlight",
  "Ecosystem": "Community of organisms and their environment"
}
```

**Quiz (JSON):**
```json
[
  {
    "question": "What is the process called?",
    "options": ["Photosynthesis", "Respiration", "Fermentation", "Digestion"],
    "correctAnswer": 0
  }
]
```

---

## 🐛 Troubleshooting

### Issue: "Firebase is not initialized"
**Solution:** Check your `.env.local` file has all Firebase values

### Issue: Chapters not showing
**Solution:** 
- Make sure you're logged in as admin
- Check Firestore has chapter documents
- Verify class and subject are selected

### Issue: Google Sign-In not working
**Solution:**
- Add your Vercel domain to Firebase Authentication → Authorized domains
- Example: `your-project.vercel.app`

### Issue: Can't login as admin
**Solution:** Use exact credentials:
- ID: `p936543773`
- Password: `9365437723`

### Issue: "You don't have permission to access this document"
**Solution:** Check Firestore Security Rules are set correctly

---

## 🔒 Security

### Before Production

1. Change default admin credentials
2. Update Firestore security rules
3. Enable email verification
4. Use HTTPS (Vercel does this automatically)
5. Never commit `.env.local` to git

### Default Credentials (Change These!)

The admin credentials provided are for initial setup only. In production:

1. Create new admin account through code
2. Remove hardcoded credentials
3. Use strong passwords

---

## 📈 Next Steps

After deployment:

1. ✅ Test login/signup
2. ✅ Login as admin
3. ✅ Add first chapter
4. ✅ Test student portal
5. ✅ Share link with users
6. ✅ Add more content
7. ✅ Monitor user analytics

---

## 🎨 Customization

### Change School Name
Search for "Pankaj Sir" in code and replace with your school name

### Change Colors
Main colors in `app/page.jsx`:
- `emerald-*` = Green (primary)
- `red-*` = Red (admin)
- `slate-*` = Dark background

### Add More Classes
Edit `StudentDashboard` component:
```javascript
const classes = [
  { id: '9', name: 'Class 9' },
  { id: '10', name: 'Class 10' },
  { id: '11', name: 'Class 11' }, // Add this
];
```

---

## 📞 Support

### Documentation
- [Firebase Docs](https://firebase.google.com/docs)
- [Next.js Docs](https://nextjs.org/docs)
- [Tailwind CSS Docs](https://tailwindcss.com/docs)

### Common Issues
- Check `.env.local` file exists with all values
- Verify Firebase services are enabled
- Clear browser cache and cookies
- Check browser console for errors

---

## 📄 License

This project is open source and available under the MIT License.

---

## 🙏 Credits

Built with:
- [Next.js](https://nextjs.org/)
- [Firebase](https://firebase.google.com/)
- [Tailwind CSS](https://tailwindcss.com/)
- [React](https://react.dev/)

---

## 🎉 You're All Set!

Your educational platform is ready to serve students. Start adding content and watch it grow!

**Questions?** Check the troubleshooting section or visit the docs.

**Happy Teaching! 🚀**

---

**Last Updated:** January 2026
**Version:** 1.0.0
**Status:** Production Ready ✅
