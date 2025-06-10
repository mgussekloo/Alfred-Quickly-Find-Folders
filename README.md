# Quickly Find Folders

Alfred workflow to Quickly Find Folders by partial match(es). Powered by the standard Find utility.

![Demo image](demo.gif)

# Usage
- Use the keyword *qff* followed by one or more partial folder names to start searching.
  - To quickly find ~/Projects/Demo/Workspace/Resources/Assets, you could use "qff demo assets"
  - To quickly find ~/Dropbox/Photos/2024/August/Spain, you could use "qff drop 24 spain"

- Press enter to "drill down" and start a new search, from here.
- Press command+enter to open in Finder, or option+enter to reveal in Finder.
- Use . (a single dot) to select the current directory, or .. (two dots) to select the parent directory.

# Good to know

This only finds folders. This is the intended behavior. The default search max depth is 3, meaning for every search term it searches three folders deep. The minimum length for a searchterm is 3 letters. This keeps searching fast-ish and prevents searching for short, generic terms. Feel free to configure it to your liking.

Folders prefixed with a dot (e.g. .git), vendor, node_modules, ~/Library and some Wordpress folders are ignored by the search.

# Requirements

This workflow requires JQ on your system.
You can configure the path to JQ in the workflow configuration.

- Use Homebrew to install jq with: brew install jq
- Use MacPorts to install jq with: port install jq
- Use Fink to install jq with: fink install jq
