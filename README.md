# Medical Terminology Hub 🏥

A comprehensive, interactive medical terminology learning platform designed for medical students, nursing students, and healthcare professionals. Master essential medical vocabulary with engaging flashcards across multiple medical specialties.

![Medical Terminology Hub](https://images.pexels.com/photos/4386467/pexels-photo-4386467.jpeg?auto=compress&cs=tinysrgb&w=1200&h=630&fit=crop)

## 🌟 Features

- **Interactive Flashcards**: Flip cards to reveal definitions and examples
- **Multiple Medical Specialties**: 6 comprehensive categories covering 50+ terms
- **Smart Search**: Find specific medical terms across all categories
- **Progress Tracking**: Monitor your study progress and accuracy
- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **Keyboard Shortcuts**: Navigate efficiently with keyboard controls
- **Modern UI**: Beautiful, professional interface with smooth animations

## 📚 Medical Categories

### Cardiovascular System ❤️
- Hypertension, Tachycardia, Bradycardia
- Myocardial Infarction, Angina, Atrial Fibrillation
- Ischemia, Thrombosis, and more...

### Respiratory System 🫁
- Pneumonia, Asthma, Bronchitis
- Dyspnea, Cyanosis, Emphysema
- Pleural Effusion, Pneumothorax

### Neurology 🧠
- Stroke, Seizure, Migraine
- Aphasia, Ataxia, Neuropathy

### Dermatology 🩺
- Dermatitis, Melanoma, Psoriasis
- Eczema, Urticaria

### Musculoskeletal System 🦴
- Arthritis, Osteoporosis, Fracture
- Tendinitis, Bursitis, Scoliosis

### Gastroenterology 🫃
- Gastritis, Jaundice, Appendicitis
- Cirrhosis, Peptic Ulcer

## 🚀 Live Demo

Visit the live application: [Medical Terminology Hub](https://medicalterminologycode.netlify.app)

## 🛠️ Technology Stack

- **Framework**: Astro 4.0
- **Styling**: Tailwind CSS
- **Language**: TypeScript
- **Build Tool**: Vite
- **Deployment**: Bolt Hosting

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/medical-terminology-hub.git
   cd medical-terminology-hub
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:4321`

## 🎮 Usage

### Navigation
- **Arrow Keys**: Navigate between flashcards (← Previous, → Next)
- **Spacebar/Enter**: Flip the current flashcard
- **S Key**: Shuffle the current category

### Features
- **Category Selection**: Click on specialty tabs to switch between medical categories
- **Search Function**: Type in the search box to find specific medical terms
- **Progress Tracking**: View your study statistics in real-time
- **Responsive Design**: Use on any device - desktop, tablet, or mobile

## 📁 Project Structure

```
medical-terminology-hub/
├── src/
│   ├── pages/
│   │   └── index.astro          # Main application page
│   ├── styles/
│   │   └── global.css           # Global styles and Tailwind imports
│   └── env.d.ts                 # TypeScript environment definitions
├── docs/                        # Documentation files
│   ├── DEPLOYMENT.md           # Deployment guide
│   └── FEATURES.md             # Feature documentation
├── dist/                        # Built files (generated)
├── astro.config.mjs            # Astro configuration
├── tailwind.config.mjs         # Tailwind CSS configuration
├── tsconfig.json               # TypeScript configuration
├── package.json                # Dependencies and scripts
├── CONTRIBUTING.md             # Contribution guidelines
├── LICENSE                     # MIT License
└── README.md                   # Project documentation
```

## 🎯 Educational Value

This platform helps students learn:
- **Medical Terminology**: Essential vocabulary for healthcare
- **Contextual Usage**: Real-world examples for each term
- **Specialty Knowledge**: Terms organized by medical specialty
- **Retention**: Interactive learning improves memory retention

## 🔧 Development

### Available Scripts

```bash
npm run dev          # Start development server
npm run build        # Build for production
npm run preview      # Preview production build
npm run astro        # Run Astro CLI commands
```

### Adding New Terms

To add new medical terms, edit the `medicalTermsByCategory` object in `src/pages/index.astro`:

```javascript
const medicalTermsByCategory = {
  categoryName: [
    {
      term: "Medical Term",
      definition: "Clear, concise definition",
      example: "Real-world usage example",
      difficulty: "Basic|Intermediate|Advanced"
    }
  ]
};
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Medical terminology sourced from standard medical dictionaries
- Icons from Heroicons
- Fonts from Google Fonts (Inter)
- Images from Pexels
- Built with Astro and Tailwind CSS

---

**Made with ❤️ for medical education**

*Helping future healthcare professionals master medical terminology one flashcard at a time.*