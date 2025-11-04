# Contributing to BatmanComfyFlow

Thank you for your interest in contributing to BatmanComfyFlow! This document provides guidelines for contributing workflows and improvements to this repository.

## How to Contribute

### Adding New Workflows

1. **Test Your Workflow**
   - Ensure your workflow runs successfully in ComfyUI
   - Test with different inputs to verify stability
   - Document any specific requirements (models, custom nodes, etc.)

2. **Export Your Workflow**
   - In ComfyUI, use "Save (API Format)" or "Save" to export your workflow
   - Use a descriptive filename (e.g., `text_to_3d_model.json`)
   - Avoid spaces in filenames; use underscores or hyphens instead

3. **Create a Pull Request**
   - Fork this repository
   - Add your workflow JSON file to the root directory
   - Update the README.md to include your workflow in the appropriate table
   - Include a brief description of what your workflow does
   - Add any preview images if available (optional)

### Workflow Naming Conventions

Use clear, descriptive names that indicate the workflow's purpose:

- **Good**: `img2img_upscale_4x.json`, `anime_video_interpolation.json`
- **Avoid**: `workflow1.json`, `test.json`, `my workflow (1).json`

### Documentation Requirements

When adding a workflow, please include in your PR description:

1. **Purpose**: What does this workflow do?
2. **Requirements**:
   - Which models are needed?
   - Any custom nodes required?
   - Minimum VRAM requirements?
3. **Use Case**: When should someone use this workflow?
4. **Example**: If possible, provide an example output or use case

### README Updates

Add your workflow to the appropriate section in README.md:

```markdown
| **your_workflow.json** | Brief description | Use case |
```

### Code of Conduct

- Be respectful and constructive
- Focus on helping others create great content
- Share knowledge and best practices
- Credit original workflow creators when adapting existing work

## Quality Guidelines

### Workflow Requirements

- **Functional**: Must run without errors in latest ComfyUI
- **Documented**: Key parameters should have clear descriptions
- **Optimized**: Remove unused nodes before exporting
- **Tested**: Verify it works with commonly available models

### File Organization

- Keep workflow files in the root directory
- Place preview images in the root (PNG format preferred)
- Use descriptive names for all files
- Avoid duplicate files

## Reporting Issues

If you find issues with existing workflows:

1. Open a GitHub issue
2. Describe the problem clearly
3. Include:
   - Which workflow file
   - ComfyUI version
   - Error messages or screenshots
   - Steps to reproduce

## Suggesting Improvements

We welcome suggestions for:

- Documentation improvements
- Workflow optimizations
- Better organization
- Additional examples or tutorials

Open an issue with the "enhancement" label to suggest improvements.

## Pull Request Process

1. **Fork & Clone**: Fork the repository and clone it locally
2. **Create Branch**: Create a feature branch (`git checkout -b add-my-workflow`)
3. **Make Changes**: Add your workflow and update documentation
4. **Test**: Verify your workflow file is valid JSON and works in ComfyUI
5. **Commit**: Write clear commit messages
   ```
   Add text-to-3D workflow with NeRF integration

   - Added text_to_3d_nerf.json workflow
   - Updated README with workflow description
   - Includes preview image
   ```
6. **Push**: Push to your fork
7. **PR**: Open a pull request with a clear description

### PR Checklist

- [ ] Workflow file added with descriptive name
- [ ] README.md updated with workflow entry
- [ ] No spaces in filenames
- [ ] Workflow tested in ComfyUI
- [ ] Preview image added (if applicable)
- [ ] Required models/nodes documented
- [ ] PR description explains the workflow

## Questions?

If you have questions about contributing:

- Open a GitHub issue with the "question" label
- Check existing issues for similar questions
- Review the README for basic usage information

## License

By contributing to this repository, you agree that your contributions will be licensed under the MIT License (see LICENSE file).

---

Thank you for helping make BatmanComfyFlow better! 🦇
