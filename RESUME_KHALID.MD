# Portfolio of Mr. Khalid Rizvi

This is a Jekyll-based portfolio showcasing the extensive technical skills and experiences of Mr. Khalid Rizvi. It's
designed to be interactive and is hosted on GitHub Pages.

## How to Use

This Jekyll theme uses data files to populate information on the site. Here's how you can customize these:

1. **Clone the repository**: Clone this repository to your local machine.

2. **Install dependencies**: Install the necessary dependencies by running `bundle install` in your terminal.

3. **Run Jekyll**: Start the Jekyll server by running `bundle exec jekyll serve` in your terminal.

4. **Open your browser**: Open `localhost:4000` in your browser to see the site.

### Additional Branches

There are two additional branches, `dxc` and `aws`, which you might need to use depending on your specific needs:

- **DXC**: If you're working on a specific project named "dxc", switch to the `dxc` branch by running `git checkout dxc`
  in your terminal before starting your work.

- **AWS**: If you're deploying the site on Amazon Web Services (AWS), switch to the `aws` branch by
  running `git checkout aws` in your terminal before starting. After you're done, sync the `_site` directory to your S3
  bucket with `aws s3 sync _site s3://khalidrizvi.com --profile munnoo`.

### Customizing Your Data

All data files are located in the `_data` directory and are written in YAML format. Here's what each file is for:

- `associations.yml`: Contains information about professional associations or groups.
- `education.yml`: Stores data about your educational background.
- `experience.yml`: Lists your work experience.
- `interests.yml`: Shares your hobbies or interests.
- `links.yml`: Contains hyperlinks to your profiles on other sites.
- `projects.yml`: Showcases projects you've worked on.
- `recognitions.yml`: Contains any awards or recognitions you've received.
- `skills.yml`: Contains a list of your skills.

Customize these files with your own information to personalize your site.

### Customizing the Configuration

The `_config.yml` file in the root directory is used to store site-wide configuration data. Here's how you can modify
it:

- **Site settings**: The `title` and `description` fields are used to set the site's title and description,
  respectively.

- **Resume settings**: These settings control the appearance of your resume. You can set your avatar, name, title,
  contact information, and introduction here. The `resume_looking_for_work` field determines whether a "Contact me"
  button is shown.

- **Section settings**: These settings control which sections are displayed on the resume. Set the corresponding field
  to `true` to display a section, or `false` to hide it.

- **Social links**: These settings control the social links displayed on the resume. Add your own URLs to display them.

- **Design settings**: The `resume_theme` field controls the theme of the resume. Currently, the only available theme
  is `default`.

### Customizing the Layout

The structure of the portfolio is defined in the `_layouts/resume.html` file. This HTML file uses Liquid templating
language to pull data from your `_config.yml` and `_data` files and display it on the page. Here's how you can modify
it:

- **Modify the sections**: Each section of the resume (e.g., Experience, Education, Projects) is enclosed in
  a `<section>` tag. You can modify these sections to customize the structure of the resume. For example, you might want
  to add a new section, change the order of sections, or modify the HTML within a section to change how it's displayed.

- **Modify the elements**: Within each section, you can modify the elements (e.g., headings, paragraphs, lists) to
  customize the content of the resume. For example, you might want to change the heading level of a title, add a new
  paragraph, or modify a list.

- **Modify the schema**: The resume uses Schema.org markup to provide additional context to search engines. You can
  modify the `itemscope` and `itemtype` attributes to change the schema. For example, you might want to add a
  new `itemscope` to a section, or change the `itemtype` of an element.

Remember, any changes you make to the `_layouts/resume.html` file will be reflected across the entire site, since this
file defines the layout for all pages.

