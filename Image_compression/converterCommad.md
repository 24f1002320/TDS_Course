
# Convert to WebP
cwebp -q 85 images/input.jpg -o images/output.webp

# Optimize PNG
pngquant --quality=65-80 image.png

# Optimize JPEG
jpegoptim --strip-all --all-progressive --max=85 image.jpg

# Convert and resize
convert input.jpg -resize 800x600 output.jpg

# Batch convert
mogrify -format webp -quality 85 *.jpg