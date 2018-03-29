TOOL_LIB = /Users/donblas/Downloads/swift
TOOL = $(TOOL_LIB)/bin/tom-swifty.exe
SWIFT_BIN_PATH = $(TOOL_LIB)/bin/swift/bin
SWIFT_LIB_PATH = $(TOOL_LIB)/bin/swift/lib/swift/macosx
SWIFT_GLUE_PATH = $(TOOL_LIB)/lib/mac/XamGlue.framework

ifeq ($(FRAMEWORK_NAME),)
FRAMEWORK_NAME = TinyConstraints
endif

all::
	mono --debug $(TOOL) --verbose --retain-swift-wrappers --swift-bin-path $(SWIFT_BIN_PATH) --swift-lib-path $(SWIFT_LIB_PATH) -o tsout -C $(FRAMEWORK_NAME).framework -C $(SWIFT_GLUE_PATH) $(FRAMEWORK_NAME)

