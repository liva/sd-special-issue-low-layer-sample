TOSHOKAN_VERSION:=v0.10
HAKASE_SOURCE:=shared.h hakase.cc
FRIEND_SOURCE:=shared.h friend.cc

TOOLS_DIR?=.misc
$(shell docker run --rm -v $(CURDIR):$(CURDIR) livadk/toshokan_tools:$(TOSHOKAN_VERSION) rsync -av /usr/local/share/misc/toshokan/ $(CURDIR)/.misc/ > /dev/null 2>&1)
include $(TOOLS_DIR)/build_rules.mk
