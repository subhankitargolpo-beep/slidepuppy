Problem: Creating a high-quality presentation is a fragmented, two-part struggle. Manually researching, structuring, and writing content for a full deck is slow and difficult.
Even after content is generated, fine-tuning the design, finding relevant media, and applying consistent branding slide-by-slide is a tedious, non-AI-assisted process in traditional software.

I built SlidePuppy, a comprehensive SaaS ecosystem that solves both problems with a unique, two-app architecture:
I developed an AI agent-based system. A user provides a single prompt (topic, audience, difficulty), and a team of specialized AI agents (Research, Structuring, Refining) collaborates to generate a complete, structured .pptx presentation. It also automatically creates a companion PDF worksheet.

I built a full-featured, AI-powered slide editor using fabric.js. This app loads the generated presentation (via IndexedDB) and acts as an "AI co-designer." It allows for granular, slide-by-slide commands (e.g., "edit this slide," "apply this theme to all slides") and uses AI to find relevant media, bridging the gap between raw generation and a polished final product.

AI Generation Agent System: A multi-agent (Research, Structure, Refine) workflow for end-to-end .pptx content creation from a single prompt.

Companion Worksheet Generator: Automatically generates and exports a PDF worksheet (jspdf/html2canvas) based on the presentation content.

Advanced AI Designer: A fabric.js canvas editor for granular, prompt-based edits (e.g., "change theme," "re-write this slide").

AI-Powered Media Search: "Magic Search" uses Gemini to analyze slide text and find relevant images/vectors via the Google Search API.

Full Export Suite: Exports to .pptx (from both the generator and designer) and .pdf.

SaaS Infrastructure: Manages API keys and uses IndexedDB to seamlessly transfer large presentation data between the generator and designer apps.

And as a client-side application, your sensitive data stays in browser.
