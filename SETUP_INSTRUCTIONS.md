# 🐍 GitHub Profile Snake Setup Instructions

Follow these steps to add the snake animation that eats your contribution graph to your GitHub profile!

## Step 1: Create Your Profile Repository

1. Create a new repository on GitHub with the **exact same name as your username**
   - For example, if your username is `johndoe`, create a repository named `johndoe`
   - Make sure it's **public**
   - Initialize it with a README

## Step 2: Add the Workflow File

1. In your profile repository, create the directory structure: `.github/workflows/`
2. Copy the `snake.yml` file from this repository to `.github/workflows/snake.yml`
3. The workflow will automatically:
   - Run every 12 hours
   - Generate snake animations from your contribution graph
   - Create both light and dark mode versions
   - Push the generated files to an `output` branch

## Step 3: Update the README

1. Replace `YOUR_USERNAME` in the `README.md` file with your actual GitHub username
2. Copy the updated README.md to your profile repository

## Step 4: Enable GitHub Actions

1. Go to your profile repository on GitHub
2. Click on the "Actions" tab
3. If prompted, enable GitHub Actions for your repository

## Step 5: Enable GitHub Pages (Optional but Recommended)

1. Go to your repository Settings
2. Scroll down to "Pages" in the left sidebar
3. Under "Source", select "Deploy from a branch"
4. Choose the `output` branch (this will be created after the first workflow run)
5. Leave the folder as `/ (root)`

## Step 6: Run the Workflow

1. Go to the "Actions" tab in your repository
2. Click on "Generate Snake Animation" workflow
3. Click "Run workflow" to trigger it manually for the first time
4. Wait for it to complete (should take 1-2 minutes)

## Step 7: Verify It's Working

1. After the workflow completes, check that an `output` branch was created
2. Your profile README should now display the snake animation!
3. The snake will automatically update every 12 hours

## Customization Options

You can customize the snake by modifying the workflow file:

- **Snake color**: Change `color_snake=orange` to any hex color
- **Dot colors**: Modify the `color_dots` parameter with 5 comma-separated colors
- **Update frequency**: Change the cron schedule in the workflow
- **Output formats**: Add or remove SVG/GIF outputs

## Troubleshooting

### Snake not appearing?
- Make sure your repository name matches your username exactly
- Check that the workflow ran successfully in the Actions tab
- Verify that the `output` branch was created
- Ensure your repository is public

### Workflow failing?
- Check that GitHub Actions are enabled
- Make sure you have the correct permissions set
- Verify the workflow file syntax is correct

### Need to update manually?
- Go to Actions → Generate Snake Animation → Run workflow

## Example URLs

After setup, your snake files will be available at:
- Light mode: `https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_USERNAME/output/github-contribution-grid-snake.svg`
- Dark mode: `https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_USERNAME/output/github-contribution-grid-snake-dark.svg`
- GIF version: `https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_USERNAME/output/github-contribution-grid-snake.gif`

---

**That's it! Your snake should now be happily eating your contribution graph! 🐍✨**