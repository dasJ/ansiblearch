# Netctl profile generator

This role will generate netctl profiles in the default directory.
Allmost all variables are directly passed into the profile.

Unit can be started/enabled using the `service` module.

## Variables

### For this role
- `netctl_profile_name` - Filename of the new profile (relative to `/etc/netctl`)

### Passed to the profile
- `netctl_profile_description` - `Description` option
- `netctl_profile_connection` - `Connection` option
- `netctl_profile_interface` - `Interface` option
- `netctl_profile_bindstointerfaces` - `BindsToInterfaces` option (array)
- `netctl_profile_after` - `After` option
- `netctl_profile_execuppost` - `ExecUpPost` option
- `netctl_profile_execdownpre` - `ExecDownPre` option
- `netctl_profile_timeoutup` - `TimeoutUp` option
- `netctl_profile_forceconnect` - `ForceConnect` option
- `netctl_profile_excludeauto` - `ExcludeAuto` option
- `netctl_profile_debug` - `NETCTL_DEBUG` option
- `netctl_profile_ip` - `IP` option
- `netctl_profile_ip6` - `IP6` option
- `netctl_profile_addresses` - `Address` option (array)
- `netctl_profile_gateway` - `Gateway` option
- `netctl_profile_routes` - `Routes` option (array)
- `netctl_profile_addresses6` - `Address6` option (array)
- `netctl_profile_gateway6` - `Gateway6` option
- `netctl_profile_routes6` - `Routes6` option (array)
- `netctl_profile_dhcpclient` - `DHCPClient` option
- `netctl_profile_dhcp6client` - `DHCP6Client` option
- `netctl_profile_dhcpreleaseonstop` - `DHCPReleaseOnStop` option
- `netctl_profile_ipcustom` - `IPCustom` option (array)
- `netctl_profile_hostname` - `Hostname` option
- `netctl_profile_dns` - `DNS` option (array)
- `netctl_profile_dnsdomain` - `DNSDomain` option
- `netctl_profile_dnssearch` - `DNSSearch` option
- `netctl_profile_dnsoptions` - `DNSOptions` option (array)
- `netctl_profile_timeoutdhcp` - `TimeoutDHCP` option
- `netctl_profile_timeoutdad` - `TimeoutDAD` option
- `netctl_profile_skipdad` - `SkipDAD` option
- `netctl_profile_auth8021x` - `Auth8021X` option
- `netctl_profile_wpaconfigfile` - `WPAConfigFile` option
- `netctl_profile_wpadriver` - `WPADriver` option
- `netctl_profile_timeoutwpa` - `TimeoutWPA` option
- `netctl_profile_skipnocarrier` - `SkipNoCarrier` option
- `netctl_profile_priority` - `Priority` option
- `netctl_profile_security` - `Security` option
- `netctl_profile_essid` - `ESSID` option
- `netctl_profile_ap` - `AP` option
- `netctl_profile_key` - `Key` option
- `netctl_profile_hidden` - `Hidden` option
- `netctl_profile_adhoc` - `AdHoc` option
- `netctl_profile_scanfrequencies` - `ScanFrequencies` option
- `netctl_profile_frequency` - `Frequency` option
- `netctl_profile_wpaconfigsection` - `WPAConfigSection` option (array)
- `netctl_profile_country` - `Country` option
- `netctl_profile_wpagroup` - `WPAGroup` option
- `netctl_profile_rfkill` - `RFKill` option
- `netctl_profile_mode` - `Mode` option
- `netctl_profile_skipforwardingdelay` - `SkipForwardingDelay` option
- `netctl_profile_user` - `User` option
- `netctl_profile_password` - `Password` option
- `netctl_profile_connectionmode` - `ConnectionMode` option
- `netctl_profile_idletimeout` - `IdleTimeout` option
- `netctl_profile_maxfail` - `MaxFail` option
- `netctl_profile_defaultroute` - `DefaultRoute` option
- `netctl_profile_usepeerdns` - `UsePeerDNS` option
- `netctl_profile_pppunit` - `PPPUnit` option
- `netctl_profile_lcpechointerval` - `LCPEchoInterval` option
- `netctl_profile_lcpechofailure` - `LCPEchoFailure` option
- `netctl_profile_optionsfile` - `OptionsFile` option
- `netctl_profile_pppoeservice` - `PPPoEService` option
- `netctl_profile_pppoeac` - `PPPoEAC` option
- `netctl_profile_pppoesession` - `PPPoESession` option
- `netctl_profile_pppoemac` - `PPPoEMAC` option
- `netctl_profile_pppoeipv6` - `PPPoEIP6` option
- `netctl_profile_accesspointname` - `AccessPointName` option
- `netctl_profile_pin` - `Pin` option
- `netctl_profile_phonenumber` - `PhoneNumber` option
- `netctl_profile_mode` - `Mode` option
- `netctl_profile_init` - `Init` option
- `netctl_profile_chatscript` - `ChatScript` option
- `netctl_profile_local` - `Local` option
- `netctl_profile_remote` - `Remote` option
- `netctl_profile_user` - `User` option
- `netctl_profile_group` - `Group` option
- `netctl_profile_vlanid` - `VLANID` option
- `netctl_profile_macaddress` - `MACAddress` option
