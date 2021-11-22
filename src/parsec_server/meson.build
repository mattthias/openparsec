
include_dirs = include_directories('../libparsec/include', '../parsec_server/include', '../parsec/include')

ncurses_dep = dependency('ncurses', version: '>=5') 

sources = [
'con_act_sv.cpp', 
'con_aux_sv.cpp', 
'con_com_sv.cpp', 
'con_ext_sv.cpp', 
'con_info_sv.cpp', 
'con_int_sv.cpp', 
'con_list_sv.cpp', 
'con_load_sv.cpp', 
'con_main_sv.cpp', 
'con_std_sv.cpp', 
'e_colldet_sv.cpp', 
'e_connmanager.cpp', 
'e_gameserver.cpp', 
'e_global_sv.cpp', 
'e_packethandler.cpp', 
'e_simnetinput.cpp', 
'e_simnetoutput.cpp', 
'e_simplayerinfo.cpp', 
'e_simulator.cpp', 
'e_world.cpp', 
'g_main_sv.cpp', 
'g_player.cpp', 
'g_stgate_sv.cpp', 
'inp_main_sv.cpp', 
'MasterServer.cpp', 
'MasterServerItem.cpp', 
'net_packetdriver.cpp', 
'net_util_sv.cpp', 
'nl_udpdriver.cpp', 
'sl_util_sv.cpp', 
'sv_main.cpp', 
'sys_err_sv.cpp', 
'sys_msg_sv.cpp', 
'sys_util_sv.cpp']

libparsec_sources = [
'../libparsec/con_arg.cpp',
'../libparsec/con_tab.cpp',
'../libparsec/con_vald.cpp',
'../libparsec/debug.cpp',
'../libparsec/e_modulemanager.cpp',
'../libparsec/e_relist.cpp',
'../libparsec/g_emp.cpp',
'../libparsec/g_extra.cpp',
'../libparsec/g_telep.cpp',
'../libparsec/net_pckt_gmsv.cpp',
'../libparsec/net_stream.cpp',
'../libparsec/net_swap.cpp',
'../libparsec/net_util.cpp',
'../libparsec/net_wrap.cpp',
'../libparsec/obj_clas.cpp',
'../libparsec/obj_creg.cpp',
'../libparsec/obj_cust.cpp',
'../libparsec/obj_odt.cpp',
'../libparsec/obj_type.cpp',
'../libparsec/sl_path.cpp',
'../libparsec/sl_timer.cpp',
'../libparsec/sw_path.cpp',
'../libparsec/sw_timer.cpp',
'../libparsec/sys_date.cpp',
'../libparsec/sys_file.cpp',
'../libparsec/sys_swap.cpp',
'../libparsec/utl_bsp.cpp',
'../libparsec/utl_clip.cpp',
'../libparsec/utl_clpo.cpp',
'../libparsec/utl_cull.cpp',
'../libparsec/utl_logfile.cpp',
'../libparsec/utl_math2.cpp',
'../libparsec/utl_math.cpp'
]

#libparsec = library('parsec', 
#                    libparsec_sources,
#                    include_directories : include_dirs,
#                    dependencies: ncurses_dep,
#                    cpp_args : '-DPARSEC_SERVER')


executable('parsec_server', 
          [sources,libparsec_sources],
          include_directories : include_dirs,
          dependencies: ncurses_dep,
          cpp_args: '-DPARSEC_SERVER'
          )


