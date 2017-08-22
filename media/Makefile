TARGET=Textures.xbt
TARGET_CURIAL=curial.xbt
TARGET_FLAT=flat.xbt

all: $(TARGET) $(TARGET_CURIAL) $(TARGET_FLAT)

.PHONY: force

$(TARGET):
	/mnt/package/mediacenter-osmc/src/xbmc-7781e47f997b2b100957c0eee2622df7346eb0e5/tools/depends/native/TexturePacker/bin/TexturePacker -dupecheck -input . -output $(TARGET)

$(TARGET_CURIAL):
	/mnt/package/mediacenter-osmc/src/xbmc-7781e47f997b2b100957c0eee2622df7346eb0e5/tools/depends/native/TexturePacker/bin/TexturePacker -dupecheck -input ../themes/curial -output $(TARGET_CURIAL)

$(TARGET_FLAT):
	/mnt/package/mediacenter-osmc/src/xbmc-7781e47f997b2b100957c0eee2622df7346eb0e5/tools/depends/native/TexturePacker/bin/TexturePacker -dupecheck -input ../themes/flat -output $(TARGET_FLAT)

clean:
	rm -f $(TARGET)
	rm -f $(TARGET_CURIAL)
	rm -f $(TARGET_FLAT)

distclean: clean
