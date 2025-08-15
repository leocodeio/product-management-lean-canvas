# Product Management Study Resources

This directory contains study materials and tools for product management.

## Files

### 01-lean-canvas.html
Interactive Lean Canvas tool with the following features:

#### Core Features
- **9-section lean canvas**: Problem, Solution, Unique Value Proposition, Unfair Advantage, Customer Segments, Key Metrics, Channels, Cost Structure, Revenue Streams
- **Rich text formatting**: Bold, italic, underline, colors, font sizes, text alignment, bullet/numbered lists
- **Auto-save**: Automatically saves your work to browser localStorage
- **Responsive design**: Works on desktop, tablet, and mobile devices

#### Export/Import Features
- **PDF Export**: High-quality PDF download using the startup name as filename
- **JSON Export/Import**: Complete data preservation with all formatting intact

#### JSON Format Structure
The JSON export format preserves all canvas data including rich text formatting:

```json
{
  "exportedAt": "2025-01-15T10:30:00.000Z",
  "version": "1.0",
  "metadata": {
    "designedFor": "Startup Name",
    "designedBy": "Designer Names",
    "date": "2025-01-15",
    "version": "1.0"
  },
  "sections": {
    "problem": {
      "content": "<b>HTML formatted content</b>",
      "existingAlternatives": "Alternative solutions"
    },
    "solution": {
      "content": "Top 3 features"
    },
    "uniqueValueProposition": {
      "content": "UVP content",
      "highLevelConcept": "High level concept"
    },
    "unfairAdvantage": {
      "content": "Unfair advantage description"
    },
    "customerSegments": {
      "content": "Target customers",
      "earlyAdopters": "Early adopter description"
    },
    "keyMetrics": {
      "content": "Key metrics to measure"
    },
    "channels": {
      "content": "Customer acquisition channels"
    },
    "costStructure": {
      "content": "Fixed and variable costs"
    },
    "revenueStreams": {
      "content": "Revenue sources"
    }
  }
}
```

#### Usage Instructions

##### Exporting from Lean Canvas
1. Click the download button (📥) in the formatting toolbar
2. Select "Download JSON" from the dropdown menu
3. The file will be automatically downloaded with your startup name as the filename

##### Importing to Lean Canvas
1. Click the upload button (📤) in the formatting toolbar
2. Select your JSON file
3. The canvas will be automatically populated with your data including all rich text formatting

#### Advantages of JSON Format
- **Complete formatting preservation**: All rich text formatting (bold, italic, colors, etc.) is maintained
- **Reliable parsing**: No complex text parsing issues
- **Native JavaScript support**: Fast and error-free import/export
- **Extensible**: Easy to add new features and data fields
- **Compact**: Efficient storage format

#### File Naming Convention
- Format: `[startup-name]-lean-canvas.json`
- Example: `spectralapp-lean-canvas.json`
- Replace spaces with hyphens
- Use lowercase for filenames

### Browser Compatibility
- Chrome/Chromium browsers (recommended)
- Firefox
- Safari
- Edge

### Dependencies
- Font Awesome icons (CDN)
- jsPDF library for PDF generation
- html2canvas for PDF rendering

### Notes
- HTML formatting from the rich text editor is preserved in JSON export/import
- Auto-save functionality uses localStorage for persistence
- Always backup your canvas data before importing new files
- The JSON format is version-controlled for future compatibility