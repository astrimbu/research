---
title: Neovim
---

Modern, community-chosen fork of vim.  

kickstart.nvim works as a launch point.  

### Autocomplete
- nvim $home\AppData\local\nvim\init.lua
	- :Mason
		- Install relevant LSPs (Language Server Protocol)
	- Note: Lua autocomplete works out of the box
		- Search 'stylua' (Lua LSP), append your LSPs in same spots:
			- local servers
			- vim.list_extend(ensure_installed)
			- formatters_by_ft
	- :checkhealth mason
		- Fix any WARNINGS / ERRORS
			- Update MSYS2 (msys64, ucrt64)
				- pacman -Suy
			- Manually install missing packages
				- https://packages.msys2.org/queue
				- e.g. pacman -Sy mingw-w64-ucrt-x86_64-7zip
			- Check PATH
				- C:\\msys64\\ucrt64\\bin
				- C:\\msys64\\usr\\bin
			- Check PowerShell version
				- $PSVersionTable
				- winget install --id Microsoft.PowerShell --source winget
