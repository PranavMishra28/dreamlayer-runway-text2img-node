# Runway Text2Img Node Screenshots

This directory contains screenshots and documentation for the Runway Text2Img node implementation.

## Files

### Screenshots
- `runway_node_ui_screenshot.png` - ComfyUI interface showing the Runway node in the node library
- `runway_sample_image.png` - Example of a generated image from the node
- `runway_node_workflow.png` - Visual diagram of the node workflow

### Documentation
- `runway_api_logs.txt` - Sample API interaction logs showing the generation process
- `runway_node_workflow.txt` - ASCII diagram of the node workflow

## Usage Instructions

1. **Setup**: Add `RUNWAY_API_KEY=sk-...` to your `.env` file
2. **Find Node**: Navigate to Node Library → api node → image → runway → "Runway Text to Image"
3. **Configure**: Set parameters:
   - `promptText`: Your image description
   - `ratio`: Choose from 9 aspect ratios (default: 1024:1024)
   - `seed`: Optional reproducibility (default: -1 for random)
   - `timeout`: Max wait time in seconds (default: 120)
4. **Generate**: Connect to workflow and run

## API Integration

The node integrates with the official Runway Gen-4 API:
- Endpoint: `https://api.dev.runwayml.com/v1/text_to_image`
- API Version: 2024-11-06
- Features: Task polling, progress tracking, error handling
- Output: ComfyUI-compatible image tensors

## Screenshots Source

The screenshots were taken from a live ComfyUI instance running locally:
- Server: `python3 ComfyUI/main.py --listen 0.0.0.0 --port 8188 --cpu`
- Browser: `http://localhost:8188`
- Node Category: api node > image > runway