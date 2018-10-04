wcd-core-objs := wcd9xxx-rst.o wcd9xxx-core-init.o wcd9xxx-core.o \
		 wcd9xxx-irq.o wcd9xxx-slimslave.o wcd9xxx-utils.o \
		 wcd9335-regmap.o wcd9335-tables.o msm-cdc-pinctrl.o \
		 msm-cdc-supply.o
obj-$(CONFIG_WCD9XXX_CODEC_CORE) += wcd-core.o

snd-soc-wcd9xxx-v2-objs := wcd9xxx-common-v2.o wcd9xxx-resmgr-v2.o wcdcal-hwdep.o \
			   wcd9xxx-soc-init.o wcd-dsp-utils.o wcd-dsp-mgr.o
obj-$(CONFIG_SND_SOC_WCD9XXX_V2) += snd-soc-wcd9xxx-v2.o
ifeq ($(CONFIG_COMMON_CLK_MSM), y)
	snd-soc-wcd9xxx-v2-objs += audio-ext-clk.o
endif
ifeq ($(CONFIG_COMMON_CLK_QCOM), y)
	snd-soc-wcd9xxx-v2-objs += audio-ext-clk-up.o
endif

snd-soc-wcd9335-objs := wcd9335.o
obj-$(CONFIG_SND_SOC_WCD9335) += snd-soc-wcd9335.o

snd-soc-wsa881x-objs := wsa881x.o wsa881x-tables.o wsa881x-regmap.o wsa881x-temp-sensor.o
obj-$(CONFIG_SND_SOC_WSA881X) += snd-soc-wsa881x.o

snd-soc-wsa881x-analog-objs := wsa881x-analog.o wsa881x-tables-analog.o wsa881x-regmap-analog.o
obj-$(CONFIG_SND_SOC_WSA881X_ANALOG) += snd-soc-wsa881x-analog.o

snd-soc-msm-stub-objs := msm_stub.o
obj-$(CONFIG_SND_SOC_MSM_STUB) += snd-soc-msm-stub.o

snd-soc-wcd-cpe-objs := wcd_cpe_core.o wcd_cpe_services.o
obj-$(CONFIG_SND_SOC_WCD_CPE) += snd-soc-wcd-cpe.o

snd-soc-wcd-spi-objs := wcd-spi.o
obj-$(CONFIG_SND_SOC_WCD_SPI) += snd-soc-wcd-spi.o

snd-soc-wcd-mbhc-objs := wcd-mbhc-v2.o
obj-$(CONFIG_SND_SOC_WCD_MBHC) += snd-soc-wcd-mbhc.o
ifeq ($(CONFIG_SND_SOC_WCD_MBHC_ADC), y)
	snd-soc-wcd-mbhc-objs += wcd-mbhc-adc.o
endif
ifeq ($(CONFIG_SND_SOC_WCD_MBHC_LEGACY), y)
	snd-soc-wcd-mbhc-objs += wcd-mbhc-legacy.o
endif

obj-$(CONFIG_SND_SOC_MSM_HDMI_CODEC_RX) += msm_hdmi_codec_rx.o
