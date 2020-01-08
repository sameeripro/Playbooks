# TCPDUMP

You can use the [editor on GitHub](https://github.com/sameeripro/Playbooks/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

## Analysis

Get domain names in DNS queries and search for suspicious TLD
```bash
`tcpdump -nn -r test.pcap dst port 53 | cut -d " " -f 8 | grep -Ev '(net|com|org)'`
```
> _-E Extended Regex -v inverted match_



```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```
`zcat -r * | grep -a "\.exe" | jq '.name' '.path'`
For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/sameeripro/Playbooks/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
