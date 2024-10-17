from pptx import Presentation
from pptx.util import Inches

# Create a presentation object
presentation = Presentation()

# Title slide
slide_title = presentation.slides.add_slide(presentation.slide_layouts[0])
title = slide_title.shapes.title
subtitle = slide_title.placeholders[1]

title.text = "Melodi Cintamu"
subtitle.text = "Lagu dengan Gaya Bahasa Penuh Emosi"

# Slide for Verse 1
slide_verse1 = presentation.slides.add_slide(presentation.slide_layouts[1])
title = slide_verse1.shapes.title
content = slide_verse1.placeholders[1]

title.text = "Verse 1"
content.text = ("Cintamu menyapa, bagai mentari berbisik,\n"
                "Pada bunga yang sedang mekar segar,\n"
                "Langit tersenyum, di saat kau mendekat,\n"
                "Mewarnai hari dengan sejuta sinar.")

# Slide for Chorus
slide_chorus = presentation.slides.add_slide(presentation.slide_layouts[1])
title = slide_chorus.shapes.title
content = slide_chorus.placeholders[1]

title.text = "Chorus"
content.text = ("Engkaulah bintang yang menari di malam,\n"
                "Menyuluh kegelapan, memberi kedamaian,\n"
                "Rinduku bagaikan ombak yang memanggil,\n"
                "Pada pantai, setiap saat tak pernah henti.")

# Slide for Verse 2
slide_verse2 = presentation.slides.add_slide(presentation.slide_layouts[1])
title = slide_verse2.shapes.title
content = slide_verse2.placeholders[1]

title.text = "Verse 2"
content.text = ("Embun pagi mencium lembut pada daun,\n"
                "Seperti cintamu yang menghangatkan,\n"
                "Awan berarak, mengiringi langkahmu,\n"
                "Menemani hari-hari penuh harapan.")

# Slide for Bridge
slide_bridge = presentation.slides.add_slide(presentation.slide_layouts[1])
title = slide_bridge.shapes.title
content = slide_bridge.placeholders[1]

title.text = "Bridge"
content.text = ("Angin membisikkan namamu, pada pohon,\n"
                "Daun-daun menari, mengekspresikan cinta,\n"
                "Pelangi tersenyum selepas hujan berlalu,\n"
                "Seperti hatiku, berseri kerana dirimu.")

# Slide for Outro
slide_outro = presentation.slides.add_slide(presentation.slide_layouts[1])
title = slide_outro.shapes.title
content = slide_outro.placeholders[1]

title.text = "Outro"
content.text = ("Bersamamu, bulan bernyanyi di langit,\n"
                "Bintang menari, menjadi saksi cinta sejati,\n"
                "Setiap detik adalah puisi yang indah,\n"
                "Alam berbicara, menyanyikan kisah kita.")

# Save the presentation
pptx_path = "/mnt/data/Melodi_Cintamu.pptx"
presentation.save(pptx_path)

pptx_path
