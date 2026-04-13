---
description: "Cancel active Ralph Wiggum loop"
allowed-tools: ["Bash(test -f .quilloom/ralph-loop.local.md:*)", "Bash(rm .quilloom/ralph-loop.local.md)", "Read(.quilloom/ralph-loop.local.md)"]
hide-from-slash-command-tool: "true"
---

# Cancel Ralph

To cancel the Ralph loop:

1. Check if `.quilloom/ralph-loop.local.md` exists using Bash: `test -f .quilloom/ralph-loop.local.md && echo "EXISTS" || echo "NOT_FOUND"`

2. **If NOT_FOUND**: Say "No active Ralph loop found."

3. **If EXISTS**:
   - Read `.quilloom/ralph-loop.local.md` to get the current iteration number from the `iteration:` field
   - Remove the file using Bash: `rm .quilloom/ralph-loop.local.md`
   - Report: "Cancelled Ralph loop (was at iteration N)" where N is the iteration value
