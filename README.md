# Quickly Find Folders

Alfred workflow to Quickly Find Folders by partial match. Powered by the standard Find utility.

![Demo image](demo.gif)

# Usage
First, configure the workflow and set a folder to start searches from. In my case, it's my development projects folder.

- Use the keyword "qff" followed by a partial folder name to start searching.
- Select a folder and press enter to "drill down" and start a search from here.
- Or select a folder and press command+enter to open in Finder, or option+enter to reveal in Finder.
- Use . (a single dot) to target the current directory, or .. (two dots) to target the parent directory.

# Good to know

The default folder maxdepth for searches is 3. The minimum length for a search query is 3 letters. These defaults aim to keep searching snappy and prevent generic results, but they can be configured to your liking.

Folders prefixed with a dot (e.g. .git), vendor, node_modules, ~/Library and some Wordpress folders are ignored by the search.

# Requirements

This workflow requires JQ on your system.
You can configure the path to JQ in the workflow configuration.

- Use Homebrew to install jq with: brew install jq
- Use MacPorts to install jq with: port install jq
- Use Fink to install jq with: fink install jq
