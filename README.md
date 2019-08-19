# Fluxus

## How to add a new post

1. Create a new file into `_posts` folder
2. Follow the bellow name convention for the file

	 `yyyy-mm-dd-post-title.md`

3. Into the recent created file, include the informations: (all informations bellow are case sensitive, be sure you are typing correctly)

  ```
  ---
  title: The post title
  author: The post author
  author-image: url-to-author-image
  date: yyyy-mm-dd
  description: The post description
  categories: category
  image: url-to-post-img
  link: url-to-post
  ---
	```

  **Note 1:** the initial and final dashes are required by Front Matter
  **Note 2:** the categories option accept one or more category separeted by single space: _e.g, category1 category2_

## How to pusblish a post

1. Be sure you saved your post file
2. On the terminal, into project folder type:

  ```
  git add .
  git commit -m 'Add The post title into blog'
  git pull
  git push
  ```

## How to create or update a category

1. Open `_includes/feed-filter.html` file
2. If you need to create a new category
  2.1. Right after que last existent category, add the code

  `<li><a href="#" class="newCategory">New Category</a></li>`

  2.2. Replace the text _newCategory_ by your category id and, _New Category_ by your category name

3. If you need to update a category
  3.1. Search for the category to be updated
  3.2. Update the class attribute and category name on HTML
  3.3. Update all the posts wich contains the previous category to the new category information
4. Update or create your post using the new or the updated category

