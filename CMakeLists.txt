
cmake_minimum_required(VERSION 2.8)

project(Plugin)

include(BroPlugin)

bro_plugin_begin(Corelight PE_XOR)
bro_plugin_cc(src/PE_XOR.cc src/Plugin.cc)
bro_plugin_bif(src/pe_xor.bif)
bro_plugin_dist_files(README CHANGES COPYING VERSION)
bro_plugin_end()
