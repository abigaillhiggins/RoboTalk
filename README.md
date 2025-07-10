# RoboTalk Blog

A blog about robotics, artificial intelligence, and technology built with Jekyll and hosted on GitHub Pages.

## Local Development

To run this blog locally:

1. Make sure you have Ruby installed:
```bash
ruby -v
```

2. Install Jekyll and Bundler:
```bash
gem install jekyll bundler
```

3. Clone this repository:
```bash
git clone https://github.com/YOUR_USERNAME/RoboTalk.git
cd RoboTalk
```

4. Install dependencies:
```bash
bundle install
```

5. Start the local server:
```bash
bundle exec jekyll serve
```

The site will be available at `http://localhost:4000/RoboTalk/`

## Creating New Posts

To create a new blog post:

1. Create a new file in the `_posts` directory with the format:
   `YYYY-MM-DD-title.md`

2. Add the front matter at the top of the file:
   ```yaml
   ---
   layout: post
   title: "Your Post Title"
   date: YYYY-MM-DD HH:MM:SS -0500
   categories: category-name
   ---
   ```

3. Write your post content in Markdown format

## Deployment

This blog is automatically deployed to GitHub Pages when changes are pushed to the main branch.

## License

This project is open source and available under the [MIT License](LICENSE). 