# Skills Directory (Legacy)

This directory contains skills that were designed for use with Amp. Since this project now uses OpenCode, these skills are no longer directly compatible.

## Legacy Status

These skills were part of the Amp ecosystem and used Amp's skill system. OpenCode uses a different approach:

- **MCP servers** for external tool integration
- **Custom commands** in `.opencode/commands/`
- **Agent configurations** in `opencode.json`

## Migration Notes

The functionality provided by these skills can be replicated using:

1. **PRD Generation**: Use OpenCode directly with prompts like:
   ```
   opencode run "Create a PRD for [your feature description]"
   ```

2. **PRD to JSON Conversion**: Use OpenCode to convert:
   ```
   opencode run "Convert tasks/prd-[feature-name].md to prd.json format following the structure in prd.json.example"
   ```

3. **Project Context**: OpenCode's `/init` command generates `AGENTS.md` automatically, which serves a similar purpose to these skills.

## Keeping These Files

These files are kept for reference purposes:
- They document the original workflow and patterns
- They may be useful for understanding the migration
- They serve as examples of how to structure similar functionality in OpenCode

If you want to remove this directory, you can safely delete it as it's no longer required for Ralph to function with OpenCode.
