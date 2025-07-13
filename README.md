# Quickly Find Folders

Alfred workflow to Quickly Find Folders by partial match(es). Powered by the standard Find utility.

![Demo image](demo.gif)

# Usage
- Use the keyword *qff* followed by one or more partial folder names to start searching.
  - To quickly find ~/Dropbox/Gusmanson/EYE/animation, use "qff drop eye anim"
  - To quickly find ~/Projects/Demo/Workspace/Resources/Assets, use "qff demo assets"
  - To quickly find ~/Backup/Photos/2024/August/Spain, use "qff back 24 spain"

- Press enter to open in Finder.
- Press command+enter to reveal in Finder, or option+enter to "drill down" and start a new search from here.
- While drilling down, search for a . (a single dot) to select the "current directory" or .. (two dots) to select the "parent directory".

# Good to know

This only finds folders by design. The default search max depth is 3, meaning for every search term it searches three folders deep. The minimum length for a searchterm is 3 letters. This keeps searching fast-ish and prevents finding too many short, generic terms. Feel free to configure it to your liking.
Folders prefixed with a dot (e.g. .git), vendor, node_modules, ~/Library and some Wordpress folders are ignored by the search.
It follows symbolic links.

# Requirements

This workflow requires JQ on your system.
You can configure the path to JQ in the workflow configuration.

- Use Homebrew to install jq with: brew install jq
- Use MacPorts to install jq with: port install jq
- Use Fink to install jq with: fink install jq
