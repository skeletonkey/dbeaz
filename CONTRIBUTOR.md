# Contributor Guidelines

Thank you for your interest in contributing to this project! This document outlines the process for contributing and the standards we expect.

## Getting Started

### 1. Fork the Repository

1. Navigate to the [main repository](https://github.com/skeletonkey/dbeaz)
2. Click the "Fork" button in the top-right corner
3. Select your GitHub account as the destination for the fork

### 2. Clone Your Fork to your computer

```bash
git clone git@github.com:YOUR_USERNAME/dbeaz.git
cd dbeaz
```

### 3. Add the Original Repository as Upstream

```bash
git remote add upstream git@github.com:skeletonkey/dbeaz.git
```

## Keeping Your Fork Updated

Before starting any new work, ensure your fork is up to date with the main repository:

```bash
# Fetch the latest changes from upstream
git fetch upstream

# Switch to your main branch
git checkout main

# Merge the upstream changes
git merge upstream/main

# Push the updates to your fork
git push origin main
```

## Creating a New Feature or Fix

### 1. Create a New Branch

Always create a new branch for your work, based off the main branch:

```bash
# Ensure you're on the main branch and it's up to date
git checkout main
git pull upstream main

# Create and switch to a new branch
git checkout -b feature/your-feature-name
# or for bug fixes:
git checkout -b fix/issue-description
```

### 2. Make Your Changes

- Write clean, readable code
- Follow existing code style and conventions
- Test your changes thoroughly
- Ensure the website works properly locally

### 3. Test Locally

**Before submitting a pull request, you must verify that:**

1. **The site works locally**: Open `index.html` in your browser and test all functionality
2. **Load times are acceptable**: Test page load times and optimize if necessary
   - Check image file sizes and use optimized versions when available
   - Minimize CSS and JavaScript if adding new files
   - Test on different connection speeds if possible
3. **All links work**: Verify internal and external links function correctly
4. **Responsive design**: Test on different screen sizes and devices
5. **Cross-browser compatibility**: Test in major browsers (Chrome, Firefox, Safari, Edge)

### 4. Commit Your Changes

```bash
# Stage your changes
git add .

# Commit with a descriptive message
git commit -m "Add feature: brief description of what you added"
```

**Commit Message Guidelines:**

- Use present tense ("Add feature" not "Added feature")
- Keep the first line under 50 characters
- Include more details in the body if necessary
- Reference issues when applicable (e.g., "Fixes #123")

### 5. Push to Your Fork

```bash
git push origin feature/your-feature-name
```

## Creating a Pull Request Using GitHub UI

1. Navigate to your fork on GitHub
2. Click "Compare & pull request" button
3. Ensure the base repository is `skeletonkey/dbeaz` and base branch is `main`
4. Ensure the head repository is your fork and compare branch is your feature branch
5. Fill out the pull request template with:
   - Clear title describing the change
   - Detailed description of what was changed and why
   - Screenshots if the change affects the UI
   - Confirmation that you've tested locally

## Code Standards

### HTML

- Use semantic HTML5 elements
- Ensure proper accessibility (alt tags, ARIA labels where needed)
- Validate HTML using W3C validator
- Use consistent indentation (2 spaces)

### CSS

- Follow existing naming conventions
- Use efficient selectors
- Optimize for performance
- Ensure responsive design
- Comment complex styles

### Images

- Optimize images for web (use optimized versions when available)
- Use appropriate formats (WebP when supported, fallback to JPEG/PNG)
- Include descriptive alt text
- Consider lazy loading for large images

### Performance

- Minimize HTTP requests
- Optimize file sizes
- Test load times on various connection speeds
- Use browser caching appropriately

## What to Include in Your PR

- [ ] Clear description of changes
- [ ] Screenshots (if UI changes)
- [ ] Confirmation that the site works locally
- [ ] Load time testing results (if applicable)
- [ ] Any new dependencies or requirements documented

## Review Process

1. All pull requests will be reviewed by maintainers
2. You may be asked to make changes or provide additional information
3. Once approved, your PR will be merged into the main branch
4. Your contribution will be acknowledged in the project

## Questions or Issues?

If you're unsure about anything or encounter issues:

1. Check existing issues and pull requests
2. Create a new issue for bugs or feature requests
3. Ask questions in your pull request if you need clarification
4. Reach out to maintainers if you need guidance

## Types of Contributions Welcome

- Bug fixes
- Performance improvements
- Accessibility enhancements
- Content updates
- Design improvements
- Documentation improvements
- Code optimization

## What Not to Include

- Large binary files (unless absolutely necessary)
- Unoptimized images
- Breaking changes without discussion
- Code that doesn't follow project conventions
- Features that significantly change the site's purpose without prior approval

---

Thank you for contributing to this project! Your efforts help make this website better for everyone.
