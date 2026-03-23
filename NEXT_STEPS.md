# Next Steps

## Done

- Selection exactly fits the pasted section after Paste
- Move tool is automatically selected after Paste
- History expanded to 100 states (up from 10)
- Sidebar widened so Simulation buttons (Step, Play, Show Next, Clear) fit on one line
- Keyboard shortcuts: Ctrl+C/V/X for Copy/Paste/Cut, Ctrl+Z/Y for Back/Forward

## Attempted But Not Working

- **Middle mouse drag for Pan** — middle mouse drag should always pan, regardless of active tool. Left mouse button behavior is still controlled by the selected tool.
- **Right mouse drag for Select** — right mouse drag should always select, regardless of active tool.
- **Undo with Draw tool** — Back/Ctrl+Z doesn't work correctly with drawn strokes. Pressing Back removes two strokes except the first dot. On a clear board with one drawn line, Back does nothing. With two lines, Back removes both except the first dot of the first line.

## To Be Done

- **Paste preview label** — in the Selection section, show a second line below the "Selected: NxN at (XX, YY)" text:
  - After copying: `To be pasted: Copied section_3x3`
  - After loading a file: `To be pasted: glider.csv`
- **Move tool preview** — when dragging with the Move tool, show a preview of where cells will land inside the red selection box. Should work correctly with Show Next (gray for moving cells, lighter pale red/blue for Show Next colors).
