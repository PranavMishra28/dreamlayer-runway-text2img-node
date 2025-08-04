To take real screenshots of the UI, generated images, and logs for the PR description, follow these steps:

1. **Start ComfyUI Server**:
   ```bash
   cd /workspaces/dreamlayer-runway-text2img-node
   python3 ComfyUI/main.py --listen 0.0.0.0 --port 8188
   ```

2. **Access the ComfyUI Interface**:
   - Open a browser and navigate to: `http://localhost:8188`
   - Create a workflow with the "Runway Text to Image" node
   - Connect inputs and outputs appropriately

3. **Take Screenshots**:
   - UI Screenshot: Capture the ComfyUI interface showing the Runway node configuration
   - Generated Image: Run the workflow and capture the resulting image
   - Logs: Capture the terminal output showing API interaction

4. **Save Screenshots**:
   Save the screenshots to:
   - `docs/images/runway_node_ui_screenshot.png`
   - `docs/images/runway_sample_image.png`
   - `docs/images/runway_logs.png`

5. **Update the PR Description**:
   - Use the content from `docs/pr_description_with_screenshots.md` as a template
   - Replace image links with your actual screenshots
   - Commit and push the images to the PR branch

Note: Since this is a dev container, you can use:
- `"$BROWSER" http://localhost:8188` to open the ComfyUI interface in your host browser
- Take screenshots using your host OS's screenshot tools
- Upload the images to GitHub directly through the PR interface
