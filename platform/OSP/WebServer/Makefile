#
# Makefile
#
# $Id: //poco/1.6/OSP/WebServer/Makefile#1 $
#
# Makefile for Poco OSP WebServer Bundle
#

BUNDLE_TOOL = $(POCO_BASE)/OSP/BundleCreator/$(POCO_HOST_BINDIR)/bundle

include $(POCO_BASE)/build/rules/global

objects = WebServerBundleActivator

target         = osp.web.server
target_version = 1
target_libs    = PocoOSPWeb PocoOSP PocoNet PocoUtil PocoXML PocoFoundation

postbuild      = $(BUNDLE_TOOL) -n$(OSNAME) -a$(OSARCH) -o../bundles WebServer.bndlspec

include $(POCO_BASE)/build/rules/dylib
