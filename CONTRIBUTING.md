# Contributing to Medical Terminology Hub

Thank you for your interest in contributing to the Medical Terminology Hub! This document provides guidelines for contributing to this educational project.

## 🎯 Project Goals

- Provide accurate, up-to-date medical terminology
- Create an engaging learning experience for medical students
- Maintain high code quality and accessibility standards
- Support multiple medical specialties

## 🚀 Getting Started

1. **Fork the repository** on GitHub
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/yourusername/medical-terminology-hub.git
   ```
3. **Install dependencies**:
   ```bash
   npm install
   ```
4. **Start the development server**:
   ```bash
   npm run dev
   ```

## 📝 How to Contribute

### Adding Medical Terms

When adding new medical terms, please follow this structure:

```javascript
{
  term: "Medical Term",
  definition: "Clear, accurate definition from medical sources",
  example: "Real-world clinical example showing usage",
  difficulty: "Basic|Intermediate|Advanced"
}
```

**Guidelines for medical terms:**
- Use authoritative medical sources
- Keep definitions concise but complete
- Provide practical clinical examples
- Classify difficulty appropriately
- Use proper medical terminology

### Code Contributions

1. **Create a feature branch**:
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. **Make your changes** following these guidelines:
   - Follow existing code style
   - Add comments for complex logic
   - Test on multiple devices
   - Ensure accessibility compliance

3. **Test your changes**:
   ```bash
   npm run build
   npm run preview
   ```

4. **Commit your changes**:
   ```bash
   git commit -m "Add: descriptive commit message"
   ```

5. **Push to your fork**:
   ```bash
   git push origin feature/your-feature-name
   ```

6. **Create a Pull Request** on GitHub

## 🎨 Design Guidelines

- **Accessibility First**: Ensure all features work with screen readers
- **Mobile Responsive**: Test on various screen sizes
- **Professional Appearance**: Maintain medical/educational aesthetic
- **Performance**: Keep load times fast
- **User Experience**: Prioritize ease of use

## 📋 Code Style

- Use TypeScript for type safety
- Follow Astro best practices
- Use Tailwind CSS for styling
- Maintain consistent indentation (2 spaces)
- Add meaningful comments
- Use semantic HTML elements

## 🧪 Testing

Before submitting a pull request:

- [ ] Test on desktop browsers (Chrome, Firefox, Safari)
- [ ] Test on mobile devices
- [ ] Verify all flashcard functionality works
- [ ] Check search functionality
- [ ] Ensure keyboard navigation works
- [ ] Validate accessibility with screen readers

## 📚 Medical Accuracy

All medical content must be:
- Verified against authoritative sources
- Reviewed for accuracy
- Appropriate for the target audience
- Free from medical advice (educational only)

## 🐛 Bug Reports

When reporting bugs, please include:
- Browser and version
- Device type (desktop/mobile/tablet)
- Steps to reproduce
- Expected vs actual behavior
- Screenshots if applicable

## 💡 Feature Requests

For new features, please:
- Check existing issues first
- Describe the educational value
- Explain the use case
- Consider implementation complexity

## 📖 Documentation

When contributing:
- Update README if needed
- Add inline code comments
- Document new features
- Update this contributing guide if necessary

## 🏥 Medical Disclaimer

This project is for educational purposes only. Contributors should:
- Not provide medical advice
- Focus on terminology education
- Cite authoritative medical sources
- Maintain educational context

## 📞 Questions?

If you have questions about contributing:
- Open an issue for discussion
- Check existing documentation
- Review similar educational projects

## 🙏 Recognition

All contributors will be recognized in the project documentation. Thank you for helping improve medical education!

---

**Remember**: This is an educational tool. Accuracy and clarity are paramount for helping future healthcare professionals learn effectively.