#
# Makefile for the memory technology device drivers.
#
# $Id: Makefile,v 1.1.1.1 2006/04/03 08:40:51 amos_lee Exp $

# Core functionality.
mtd-y				:= mtdcore.o
mtd-$(CONFIG_MTD_PARTITIONS)	+= mtdpart.o
obj-$(CONFIG_MTD)		+= $(mtd-y)

obj-$(CONFIG_MTD_CONCAT)	+= mtdconcat.o
obj-$(CONFIG_MTD_REDBOOT_PARTS) += redboot.o
obj-$(CONFIG_MTD_CMDLINE_PARTS) += cmdlinepart.o
obj-$(CONFIG_MTD_AFS_PARTS)	+= afs.o

# 'Users' - code which presents functionality to userspace.
obj-$(CONFIG_MTD_CHAR)		+= mtdchar.o
obj-$(CONFIG_MTD_BLOCK)		+= mtdblock.o mtd_blkdevs.o
obj-$(CONFIG_MTD_BLOCK_RO)	+= mtdblock_ro.o mtd_blkdevs.o
obj-$(CONFIG_FTL)		+= ftl.o mtd_blkdevs.o
obj-$(CONFIG_NFTL)		+= nftl.o mtd_blkdevs.o
obj-$(CONFIG_INFTL)		+= inftl.o mtd_blkdevs.o
obj-$(CONFIG_RFD_FTL)		+= rfd_ftl.o mtd_blkdevs.o

nftl-objs		:= nftlcore.o nftlmount.o
inftl-objs		:= inftlcore.o inftlmount.o

obj-y		+= chips/ maps/ devices/ nand/ onenand/
