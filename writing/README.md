# Writing Project Structure

This directory contains your writing projects organized as follows:

- **ideas/**: Initial concepts, seeds of inspiration, and brainstorming notes
- **drafts/**: Works in progress and ongoing writing projects
- **final/**: Completed and polished pieces ready for sharing or publication
- **resources/**: Research materials, references, and supporting documents
- **archive/**: Previous versions and older projects worth keeping

## Usage Tips

- Use the `ideas/` directory to quickly capture new concepts before they slip away
- Move work to `drafts/` when you begin developing an idea into something more substantial 
- Only move completed work to `final/` when it's ready for others to read
- Store research materials in `resources/` with clear filenames

## Version Control with Git

### Writing Workflow with Git

1. **Capturing Ideas**
   - Create a branch for each new idea: `git checkout -b idea/short-title`
   - Add files to `ideas/` directory: `git add ideas/my-new-concept.md`
   - Commit regularly: `git commit -m "Add initial concept for story"`
   - Push to share with collaborators: `git push origin idea/short-title`

2. **Developing Drafts**
   - When ready to develop an idea: `git checkout -b draft/short-title`
   - Move files from ideas to drafts: `git mv ideas/concept.md drafts/concept.md`
   - Track progress with meaningful commits: `git commit -m "Expand character development in chapter 2"`
   - Use tags for major milestones: `git tag -a "first-draft-v1" -m "Completed first draft"`

3. **Managing Resources**
   - Track research materials: `git add resources/research-notes.md`
   - Link resources to drafts with relative paths in your markdown
   - Use commit messages to document how resources inform your writing: `git commit -m "Add historical research for setting"`

4. **Finalizing Work**
   - Create a release branch: `git checkout -b release/story-title`
   - Perform final edits and formatting
   - Move to final directory: `git mv drafts/story.md final/story.md`
   - Tag completed works: `git tag -a "v1.0" -m "Final publication version"`

5. **Archiving and Revision History**
   - Archive previous versions: `git mv drafts/old-version.md archive/old-version.md`
   - View history of a piece: `git log --follow -- final/story.md`
   - Compare versions: `git diff draft-v1..draft-v2 drafts/story.md`

### Collaboration Tips

- Create pull requests for feedback before finalizing major pieces
- Use issues to track tasks, bugs, and future ideas
- Utilize branch protection to prevent accidental changes to finalized work
- Set up automated backups of your Git repository
