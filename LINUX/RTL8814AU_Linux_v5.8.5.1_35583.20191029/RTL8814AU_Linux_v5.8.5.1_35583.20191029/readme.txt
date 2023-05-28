===============================================================================
		Software Package - Component
===============================================================================
	1. ReleaseNotes.pdf

	2. document/
		Driver_Configuration_for_RF_Regulatory_Certification.pdf
		How_to_append_vendor_specific_ie_to_driver_management_frames.pdf
		How_to_set_driver_debug_log_level.pdf
		HowTo_enable_and_verify_TDLS_function_in_Wi-Fi_driver.pdf
		HowTo_enable_driver_to_support_80211d.pdf
		HowTo_enable_the_power_saving_functionality.pdf
		HowTo_support_WIFI_certification_test.pdf
		linux_dhcp_server_notes.txt
		Quick_Start_Guide_for_Adaptivity_and_Carrier_Sensing_Test.pdf
		Quick_Start_Guide_for_Bridge.pdf
		Quick_Start_Guide_for_Driver_Compilation_and_Installation.pdf
		Quick_Start_Guide_for_SoftAP.pdf
		Quick_Start_Guide_for_Station_Mode.pdf
		Quick_Start_Guide_for_WOW.pdf
		Quick_Start_Guide_for_wpa_supplicant_WiFi_P2P_test.pdf
		Realtek_WiFi_concurrent_mode_Introduction.pdf
		SoftAP_Mode_features.pdf
		Wireless_tools_porting_guide.pdf
		wpa_cli_with_wpa_supplicant.pdf
		Quick_Start_Guide_for_WPA3.pdf

	3. driver/
		3.1 rtl8814AU_linux_v5.8.5.1_35583.20191029.tar.gz
			Naming rule: rtlCHIPS_linux_vM.N.P[.H]_sssss.yyyymmdd[_COEX_VER][_beta].tar.gz
			where:
				CHIPS: supported chips
				M: Major version
				N: miNor version
				P: Patch number
				H: Hotfix number
				s: SVN number
				y: package year
				m: package month
				d: package day
				COEX_VER: Coext version
				_beta: beta driver

	4. wireless_tools/
		wireless_tools.30.rtl.tar.gz

	5. wpa_supplicant_hostapd/
		wpa_supplicant_hostapd-0.8_rtw_r24647.20171025.tar.gz
			wpa_supplicant
				The tool help the wlan network to communicate under the
				protection of WPAPSK mechanism (WPA/WPA2) and add WPS patch
			hostapd
		wpa_0_8.conf
			Configure file sample for wpa_supplicant-0.8
		rtl_hostapd_2G.conf
		rtl_hostapd_5G.conf
			Configure files for Soft-AP mode 2.4G/5G
		p2p_hostapd.conf
			Configure file for hostapd for Wi-Fi Direct (P2P)

		wpa_supplicant_8_kk_4.4_rtw_r25669.20171213.tar.gz
			wpa_supplicant_8 from Android 4.4 SDK and patched by Realtek
			could be used for pure-linux and Android 4.4. Support only cfg80211/nl80211.

		wpa_supplicant_8_L_5.x_rtw_r24600.20171025.tar.gz
			wpa_supplicant_8 from Android 5.x SDK and patched by Realtek
			could be used for pure-linux and Android 5.x. Support only cfg80211/nl80211.

		wpa_supplicant_8_O_8.x_rtw_r31832.20190226.tar.gz
			wpa_supplicant_8 from Android 8.x SDK and patched by Realtek
			could be used for pure-linux and Android 8.x. Support only cfg80211/nl80211.

		wpa_supplicant_8_P_9.x_rtw_r29226.20180827.tar.gz
			wpa_supplicant_8 from Android 9.x SDK and patched by Realtek
			could be used for Android 9.x. Support only cfg80211/nl80211.

	11. install.sh 
		Script to compile and install WiFi driver easily in PC-Linux
	
	12. User Guide for Driver compilation and installation
==================================================================================================================
			(*) Please refer to document/Quick_Start_Guide_for_Driver_Compilation_and_Installation.pdf
==================================================================================================================
		User Guide for Station mode
==================================================================================================================
			(*) Please refer to document/Quick_Start_Guide_for_Station_Mode.pdf
==================================================================================================================
		User Guide for Soft-AP mode
==================================================================================================================
			(*) Please refer to document/Quick_Start_Guide_for_SoftAP.pdf
			Soft-AP mode with Realtek's rtl871xdrv
				(*) Please use wpa_supplicant_hostapd-0.8_rtw_r24647.20171025.tar.gz
			Soft-AP mode with nl80211
				(*) Please use:
					wpa_supplicant_8_kk_4.4_rtw_r25669.20171213.tar.gz
				or
					wpa_supplicant_8_L_5.x_rtw_r24600.20171025.tar.gz
				or
					wpa_supplicant_8_O_8.x_rtw_r31832.20190226.tar.gz
			(*) Please refer to document/linux_dhcp_server_notes.txt
==================================================================================================================
		User Guide for Wi-Fi Direct
==================================================================================================================
		Wi-Fi Direct with nl80211
			(*) Please use:
					wpa_supplicant_8_kk_4.4_rtw_r25669.20171213.tar.gz
				or
					wpa_supplicant_8_L_5.x_rtw_r24600.20171025.tar.gz
				or
					wpa_supplicant_8_O_8.x_rtw_r31832.20190226.tar.gz
			(*) For P2P instruction/command, please refer to:
					README-P2P inside the wpa_supplicant folder of the wpa_supplicant_8 you choose
			(*) For DHCP server, please refer to:
					document/linux_dhcp_server_notes.txt
==================================================================================================================
		User Guide for WPS2.0
==================================================================================================================
			(*) Please use:
					wpa_supplicant_hostapd-0.8_rtw_r24647.20171025.tar.gz
				or
					wpa_supplicant_8_kk_4.4_rtw_r25669.20171213.tar.gz
				or
					wpa_supplicant_8_L_5.x_rtw_r24600.20171025.tar.gz
				or
					wpa_supplicant_8_O_8.x_rtw_r31832.20190226.tar.gz
			(*) For WPS instruction/command, please refert to:
					README-WPS inside the wpa_supplicant folder of the wpa_supplicant_8 you choose
==================================================================================================================
		User Guide for Power Saving Mode
==================================================================================================================
			(*) Please refer to document/HowTo_enable_the_power_saving_functionality.pdf
================================================================================================================
		User Guide for Applying Wi-Fi solution onto Andriod System
==================================================================================================================
			(*) For Android 1.6 ~ 2.3, 4.0, 4.1, 4.2, 4.3, 6.x, 7.x, please contact us for further information
			(*) For Android 4.4, please refer to android_ref_codes_KK_4.4/Realtek_Wi-Fi_SDK_for_Android_KK_4.4.pdf
			(*) For Android 5.x, please refer to android_ref_codes_L_5.x/Realtek_Wi-Fi_SDK_for_Android_L_5.x.pdf
			(*) For Android 8.0, please refer to android_ref_codes_O_8.0/Realtek_Wi-Fi_SDK_for_Android_O_8.0.pdf
			(*) For Android 9.x, please refer to android_ref_codes_P_9.x/Realtek_Wi-Fi_SDK_for_Android_P_9.x.pdf
==================================================================================================================
		User Guide for WPA3 Personal
==================================================================================================================
			(*) wpa_supplicant_8_O_8.x_rtw_r33457.20190507.tar.gz
			(*) Please refer to wpa_cli_with_wpa_supplicant.pdf
			(*) Please refer to Quick_Start_Guide_for_WPA3.pdf