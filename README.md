# Orgler URL Converter

## Power BI URL Creator for Story Maps & RCView Embedding

A simple tool to convert Power BI report URLs into Orgler-compatible format for embedding in ArcGIS Story Maps and RCView dashboards.

### 🔗 Live Tool
[https://franzenjb.github.io/orgler-conversion/](https://franzenjb.github.io/orgler-conversion/)

## Purpose

This tool streamlines the process of converting Power BI report URLs into the proper format needed for embedding within American Red Cross ArcGIS dashboards and Story Maps. It automatically:

- Extracts the report ID from Power BI URLs
- Preserves the report section/page information
- Maintains query parameters
- Generates the correct Orgler URL format

## How to Use

1. **Copy your Power BI URL** from the browser address bar when viewing your report
2. **Paste it** into the converter tool
3. **Click Convert** to generate the Orgler URL
4. **Copy the result** and use it in your Story Map or RCView dashboard

## URL Format

### Input (Power BI):
```
https://app.powerbi.com/groups/{group-id}/reports/{report-id}/{section}?experience=power-bi
```

### Output (Orgler):
```
https://orglerws.redcross.org/PowerBI/Home/Report/{report-id}/{section}?experience=power-bi
```

## Examples

### DSC Dashboard
- **Power BI:** `https://app.powerbi.com/groups/573e6237-a6bf-44ab-8dda-ba0c703b6791/reports/dceef683-6813-4f4c-a8f7-1cce4fac0fa2/ReportSection`
- **Orgler:** `https://orglerws.redcross.org/PowerBI/Home/Report/dceef683-6813-4f4c-a8f7-1cce4fac0fa2/ReportSection`

### REC Dashboard
- **Power BI:** `https://app.powerbi.com/groups/573e6237-a6bf-44ab-8dda-ba0c703b6791/reports/ac99ebff-5905-4d07-84db-36163ba59613/ReportSection`
- **Orgler:** `https://orglerws.redcross.org/PowerBI/Home/Report/ac99ebff-5905-4d07-84db-36163ba59613/ReportSection`

## Features

- ✅ Handles both encoded and decoded URLs
- ✅ Preserves query parameters
- ✅ Auto-converts on paste
- ✅ One-click copy to clipboard
- ✅ Mobile responsive
- ✅ Works offline once loaded

## Technical Details

- Pure HTML/CSS/JavaScript (no dependencies)
- Client-side processing only (no data sent to servers)
- American Red Cross branding and colors

## Support

For issues or questions, please contact the American Red Cross IT team or create an issue in this repository.

---

**American Red Cross** - Disaster Cycle Services Technology