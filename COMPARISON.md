# Terminal Presentation Tools Comparison

## Feature Comparison Table

| Feature | Term Deck | Slides (maaslalani) | Presenterm | Patat | mdp |
|---------|-----------|---------------------|------------|-------|-----|
| **Language** | Rust | Go | Rust | Haskell | C |
| **Markdown Support** | ✅ Basic (headers only) | ✅ Full | ✅ Full | ✅ Full (via Pandoc) | ✅ Full |
| **Slide Separator** | `<!-- end_slide -->` | `---` | `---` | `---` | `---` or `***` |
| **Metadata/Frontmatter** | ✅ YAML | ✅ Custom | ✅ YAML | ✅ YAML | ✅ Headers with @ |
| **Syntax Highlighting** | ✅ (Rust, Java, Python via tree-sitter) | ❌ | ✅ Wide language support | ✅ ~100 languages (Kate) | ❌ |
| **Live Code Execution** | ❌ | ✅ | ❌ | ✅ (code evaluation) | ❌ |
| **Images** | ✅ (via viuer) | ❌ | ✅ (kitty, iterm2, sixel, ascii) | ✅ Experimental | ❌ |
| **Animated GIFs** | ❌ | ❌ | ✅ | ❌ | ❌ |
| **Live Reload** | ❌ | ✅ | ❌ | ✅ (--watch) | ✅ (r key) |
| **SSH Serving** | ❌ | ✅ | ❌ | ❌ | ❌ |
| **PDF Export** | ❌ | ❌ | ✅ (weasyprint) | ❌ | ✅ (via md2pdf) |
| **Speaker Notes** | ❌ | ❌ | ✅ | ✅ (second window) | ❌ |
| **Themes** | ✅ 3 built-in | ✅ JSON themes | ✅ Many built-in | ✅ 24-bit RGB | ❌ (config.h) |
| **Theme Cycling** | ✅ (t key) | ❌ | ❌ | ❌ | ❌ |
| **Progressive Display** | ❌ | ❌ | ✅ (pauses) | ✅ (incremental) | ✅ (stop points) |
| **Column Layout** | ❌ | ❌ | ✅ | ❌ | ❌ |
| **Search** | ❌ | ✅ (regex) | ❌ | ❌ | ❌ |
| **Font Size Support** | ❌ | ❌ | ✅ (kitty protocol) | ❌ | ❌ |
| **Tables** | ❌ | ✅ | ✅ | ✅ | ❌ |
| **Lists** | ✅ Basic | ✅ | ✅ | ✅ | ✅ |
| **Block Quotes** | ❌ | ✅ | ✅ | ✅ | ❌ |
| **Auto-advance** | ❌ | ❌ | ❌ | ✅ | ❌ |
| **Jump to Slide** | ❌ | ❌ | ✅ (nG) | ✅ | ✅ (1..N) |
| **Text Alignment** | ❌ | ❌ | ✅ (left/center) | ✅ | ❌ |
| **Pre-processing** | ❌ | ✅ (~~~) | ❌ | ❌ | ❌ |

## Navigation Controls Comparison

| Action | Term Deck | Slides | Presenterm | Patat | mdp |
|--------|-----------|--------|------------|-------|-----|
| **Next Slide** | l | →, j, l, Space | →, j, l, PgDn | →, j, l, Space | →, j, l, Space |
| **Previous Slide** | h | ←, k, h | ←, k, h, PgUp | ←, k, h | ←, k, h, Backspace |
| **First Slide** | - | - | gg | Home | g, Home |
| **Last Slide** | - | - | G | End | G, End |
| **Jump to Slide N** | - | - | nG | - | 1..N |
| **Quit** | q | Ctrl+C | q | q | q |
| **Search** | - | / | - | - | - |
| **Reload** | - | - | - | - | r |

## Summary

### Term Deck Strengths:
- Simple and focused
- Written in Rust (memory safe, fast)
- Tree-sitter based syntax highlighting
- Theme cycling during presentation
- Image support

### Term Deck Limitations Compared to Alternatives:
- Limited markdown support (headers only)
- No live code execution
- No progressive/incremental display
- No speaker notes
- No PDF export
- No live reload
- No search functionality
- No SSH serving
- No tables or block quotes support
- Cannot jump to specific slides
- No column layout
- No auto-advance

### Most Feature-Rich Tools:
1. **Presenterm** - Most comprehensive feature set with modern capabilities
2. **Patat** - Powerful due to Pandoc integration, excellent language support
3. **Slides** - Unique features like SSH serving and live code execution

### Simplest Tool:
**mdp** - Written in C, most basic feature set but very lightweight

### Best for Learning Rust:
**Term Deck** and **Presenterm** are both Rust projects, with Term Deck being
simpler and more approachable for learning purposes.