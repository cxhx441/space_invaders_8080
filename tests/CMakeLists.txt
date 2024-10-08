
# MOV REG to REG Tests - create a unique name, use the opcode as the first argument for the executable (COMMAND function_name arg1)
add_executable(mov_reg_to_reg test_mov_reg_to_reg.c)
add_test(NAME test_mov_b_b COMMAND mov_reg_to_reg 0x40)
add_test(NAME test_mov_b_c COMMAND mov_reg_to_reg 0x41)
add_test(NAME test_mov_b_d COMMAND mov_reg_to_reg 0x42)
add_test(NAME test_mov_b_e COMMAND mov_reg_to_reg 0x43)
add_test(NAME test_mov_b_h COMMAND mov_reg_to_reg 0x44)
add_test(NAME test_mov_b_l COMMAND mov_reg_to_reg 0x45)
add_test(NAME test_mov_b_a COMMAND mov_reg_to_reg 0x47)
add_test(NAME test_mov_c_b COMMAND mov_reg_to_reg 0x48)
add_test(NAME test_mov_c_c COMMAND mov_reg_to_reg 0x49)
add_test(NAME test_mov_c_d COMMAND mov_reg_to_reg 0x4a)
add_test(NAME test_mov_c_e COMMAND mov_reg_to_reg 0x4b)
add_test(NAME test_mov_c_h COMMAND mov_reg_to_reg 0x4c)
add_test(NAME test_mov_c_l COMMAND mov_reg_to_reg 0x4d)
add_test(NAME test_mov_c_a COMMAND mov_reg_to_reg 0x4f)
add_test(NAME test_mov_d_b COMMAND mov_reg_to_reg 0x50)
add_test(NAME test_mov_d_c COMMAND mov_reg_to_reg 0x51)
add_test(NAME test_mov_d_d COMMAND mov_reg_to_reg 0x52)
add_test(NAME test_mov_d_e COMMAND mov_reg_to_reg 0x53)
add_test(NAME test_mov_d_h COMMAND mov_reg_to_reg 0x54)
add_test(NAME test_mov_d_l COMMAND mov_reg_to_reg 0x55)
add_test(NAME test_mov_d_a COMMAND mov_reg_to_reg 0x57)
add_test(NAME test_mov_e_b COMMAND mov_reg_to_reg 0x58)
add_test(NAME test_mov_e_c COMMAND mov_reg_to_reg 0x59)
add_test(NAME test_mov_e_d COMMAND mov_reg_to_reg 0x5a)
add_test(NAME test_mov_e_e COMMAND mov_reg_to_reg 0x5b)
add_test(NAME test_mov_e_h COMMAND mov_reg_to_reg 0x5c)
add_test(NAME test_mov_e_l COMMAND mov_reg_to_reg 0x5d)
add_test(NAME test_mov_e_a COMMAND mov_reg_to_reg 0x5f)
add_test(NAME test_mov_h_b COMMAND mov_reg_to_reg 0x60)
add_test(NAME test_mov_h_c COMMAND mov_reg_to_reg 0x61)
add_test(NAME test_mov_h_d COMMAND mov_reg_to_reg 0x62)
add_test(NAME test_mov_h_e COMMAND mov_reg_to_reg 0x63)
add_test(NAME test_mov_h_h COMMAND mov_reg_to_reg 0x64)
add_test(NAME test_mov_h_l COMMAND mov_reg_to_reg 0x65)
add_test(NAME test_mov_h_a COMMAND mov_reg_to_reg 0x67)
add_test(NAME test_mov_l_b COMMAND mov_reg_to_reg 0x68)
add_test(NAME test_mov_l_c COMMAND mov_reg_to_reg 0x69)
add_test(NAME test_mov_l_d COMMAND mov_reg_to_reg 0x6a)
add_test(NAME test_mov_l_e COMMAND mov_reg_to_reg 0x6b)
add_test(NAME test_mov_l_h COMMAND mov_reg_to_reg 0x6c)
add_test(NAME test_mov_l_l COMMAND mov_reg_to_reg 0x6d)
add_test(NAME test_mov_l_a COMMAND mov_reg_to_reg 0x6f)
add_test(NAME test_mov_a_b COMMAND mov_reg_to_reg 0x78)
add_test(NAME test_mov_a_c COMMAND mov_reg_to_reg 0x79)
add_test(NAME test_mov_a_d COMMAND mov_reg_to_reg 0x7a)
add_test(NAME test_mov_a_e COMMAND mov_reg_to_reg 0x7b)
add_test(NAME test_mov_a_h COMMAND mov_reg_to_reg 0x7c)
add_test(NAME test_mov_a_l COMMAND mov_reg_to_reg 0x7d)
add_test(NAME test_mov_a_a COMMAND mov_reg_to_reg 0x7f)

# MOV MEM to REG Tests - create a unique name, use the opcode as the first argument for the executable (COMMAND function_name arg1)
add_executable(test_mov_mem_to_reg test_mov_mem_to_reg.c)
add_test(NAME test_mov_b_m COMMAND test_mov_mem_to_reg 0x46)
add_test(NAME test_mov_c_m COMMAND test_mov_mem_to_reg 0x4e)
add_test(NAME test_mov_d_m COMMAND test_mov_mem_to_reg 0x56)
add_test(NAME test_mov_e_m COMMAND test_mov_mem_to_reg 0x5e)
add_test(NAME test_mov_h_m COMMAND test_mov_mem_to_reg 0x66)
add_test(NAME test_mov_l_m COMMAND test_mov_mem_to_reg 0x6e)
add_test(NAME test_mov_a_m COMMAND test_mov_mem_to_reg 0x7e)

# MOV REG to MEM Tests - create a unique name, use the opcode as the first argument for the executable (COMMAND function_name arg1)
add_executable(test_mov_reg_to_mem test_mov_reg_to_mem.c)
add_test(NAME test_mov_m_b COMMAND test_mov_reg_to_mem 0x70)
add_test(NAME test_mov_m_c COMMAND test_mov_reg_to_mem 0x71)
add_test(NAME test_mov_m_d COMMAND test_mov_reg_to_mem 0x72)
add_test(NAME test_mov_m_e COMMAND test_mov_reg_to_mem 0x73)
add_test(NAME test_mov_m_h COMMAND test_mov_reg_to_mem 0x74)
add_test(NAME test_mov_m_l COMMAND test_mov_reg_to_mem 0x75)
add_test(NAME test_mov_m_a COMMAND test_mov_reg_to_mem 0x77)

# ANA REG Tests
add_executable(test_ana_reg test_ana_reg.c)
add_test(NAME ana_b COMMAND test_ana_reg 0xa0)
add_test(NAME ana_c COMMAND test_ana_reg 0xa1)
add_test(NAME ana_d COMMAND test_ana_reg 0xa2)
add_test(NAME ana_e COMMAND test_ana_reg 0xa3)
add_test(NAME ana_h COMMAND test_ana_reg 0xa4)
add_test(NAME ana_l COMMAND test_ana_reg 0xa5)
add_test(NAME ana_m COMMAND test_ana_reg 0xa6)
add_test(NAME ana_a COMMAND test_ana_reg 0xa7)

# XRA and XRI Tests
add_executable(test_xra_xri test_xra_xri.c)
add_test(NAME xra_b COMMAND test_xra_xri 0xa8)
add_test(NAME xra_c COMMAND test_xra_xri 0xa9)
add_test(NAME xra_d COMMAND test_xra_xri 0xaa)
add_test(NAME xra_e COMMAND test_xra_xri 0xab)
add_test(NAME xra_h COMMAND test_xra_xri 0xac)
add_test(NAME xra_l COMMAND test_xra_xri 0xad)
add_test(NAME xra_m COMMAND test_xra_xri 0xae)
add_test(NAME xra_a COMMAND test_xra_xri 0xaf)
add_test(NAME xri COMMAND test_xra_xri 0xee)

# ORA and ORI Tests
add_executable(test_ora_ori test_ora_ori.c)
add_test(NAME ora_b COMMAND test_ora_ori 0xb0)
add_test(NAME ora_c COMMAND test_ora_ori 0xb1)
add_test(NAME ora_d COMMAND test_ora_ori 0xb2)
add_test(NAME ora_e COMMAND test_ora_ori 0xb3)
add_test(NAME ora_h COMMAND test_ora_ori 0xb4)
add_test(NAME ora_l COMMAND test_ora_ori 0xb5)
add_test(NAME ora_m COMMAND test_ora_ori 0xb6)
add_test(NAME ora_a COMMAND test_ora_ori 0xb7)
add_test(NAME ori COMMAND test_ora_ori 0xf6)

# Jump Tests
add_executable(test_jump test_jump.c)
add_test(NAME jnz COMMAND test_jump 0xc2)
add_test(NAME jmp COMMAND test_jump 0xc3)
add_test(NAME jz COMMAND test_jump 0xca)
add_test(NAME jnc COMMAND test_jump 0xd2)
add_test(NAME jc COMMAND test_jump 0xda)
add_test(NAME jpo COMMAND test_jump 0xe2)
add_test(NAME pchl COMMAND test_jump 0xe9)
add_test(NAME jpe COMMAND test_jump 0xea)
add_test(NAME jp COMMAND test_jump 0xf2)
add_test(NAME jm COMMAND test_jump 0xfa)

# Return Tests
add_executable(test_return test_return.c)
add_test(NAME rnz COMMAND test_return 0xc0)
add_test(NAME rz COMMAND test_return 0xc8)
add_test(NAME ret COMMAND test_return 0xc9)
add_test(NAME rnc COMMAND test_return 0xd0)
add_test(NAME rc COMMAND test_return 0xd8)
add_test(NAME rpo COMMAND test_return 0xe0)
add_test(NAME rpe COMMAND test_return 0xe8)
add_test(NAME rp COMMAND test_return 0xf0)
add_test(NAME rm COMMAND test_return 0xf8)

# Test Load Instructions
add_executable(test_load test_load.c)
add_test(NAME test_LXI_B COMMAND test_load 0x01)
add_test(NAME test_LXI_D COMMAND test_load 0x11)
add_test(NAME test_LXI_H COMMAND test_load 0x21)
add_test(NAME test_LXI_SP COMMAND test_load 0x31)
add_test(NAME test_LDAX_B COMMAND test_load 0x0a)
add_test(NAME test_LDAX_D COMMAND test_load 0x1a)
add_test(NAME test_LDA COMMAND test_load 0x3a)
add_test(NAME test_LHLD COMMAND test_load 0x2a)

add_executable(test_store test_store.c)
add_test(NAME test_SHLD COMMAND test_store 0x22)
add_test(NAME test_SPHL COMMAND test_store 0xf9)
add_test(NAME test_STA COMMAND test_store 0x32)
add_test(NAME test_STAX_B COMMAND test_store 0x02)
add_test(NAME test_STAX_D COMMAND test_store 0x12)

# Test Add Instructions
add_executable(test_add test_add.c)
add_test(NAME test_INR_A COMMAND test_add 0x3c)
add_test(NAME test_INR_B COMMAND test_add 0x04)
add_test(NAME test_INR_C COMMAND test_add 0x0c)
add_test(NAME test_INR_D COMMAND test_add 0x14)
add_test(NAME test_INR_E COMMAND test_add 0x1c)
add_test(NAME test_INR_H COMMAND test_add 0x24)
add_test(NAME test_INR_L COMMAND test_add 0x2c)
add_test(NAME test_INR_M COMMAND test_add 0x34)
add_test(NAME test_INX_B COMMAND test_add 0x03)
add_test(NAME test_INX_D COMMAND test_add 0x13)
add_test(NAME test_INX_H COMMAND test_add 0x23)
add_test(NAME test_INX_SP COMMAND test_add 0x33)
add_test(NAME test_ADD_A COMMAND test_add 0x87)
add_test(NAME test_ADD_B COMMAND test_add 0x80)
add_test(NAME test_ADD_C COMMAND test_add 0x81)
add_test(NAME test_ADD_D COMMAND test_add 0x82)
add_test(NAME test_ADD_E COMMAND test_add 0x83)
add_test(NAME test_ADD_H COMMAND test_add 0x84)
add_test(NAME test_ADD_L COMMAND test_add 0x85)
add_test(NAME test_ADD_M COMMAND test_add 0x86)
add_test(NAME adi_d8 COMMAND test_add 0xc6)
add_test(NAME test_ADC_A COMMAND test_add 0x8f)
add_test(NAME test_ADC_B COMMAND test_add 0x88)
add_test(NAME test_ADC_C COMMAND test_add 0x89)
add_test(NAME test_ADC_D COMMAND test_add 0x8a)
add_test(NAME test_ADC_E COMMAND test_add 0x8b)
add_test(NAME test_ADC_H COMMAND test_add 0x8c)
add_test(NAME test_ADC_L COMMAND test_add 0x8d)
add_test(NAME test_ADC_M COMMAND test_add 0x8e)
add_test(NAME test_ACI COMMAND test_add 0xce)
add_test(NAME test_DAD_B COMMAND test_add 0x09)
add_test(NAME test_DAD_D COMMAND test_add 0x19)
add_test(NAME test_DAD_H COMMAND test_add 0x29)
add_test(NAME test_DAD_SP COMMAND test_add 0x39)

# Test Subtract Instructions
add_executable(test_subtract test_subtract.c)
add_test(NAME test_DCR_A COMMAND test_subtract 0x3d)
add_test(NAME test_DCR_B COMMAND test_subtract 0x05)
add_test(NAME test_DCR_C COMMAND test_subtract 0x0d)
add_test(NAME test_DCR_D COMMAND test_subtract 0x15)
add_test(NAME test_DCR_E COMMAND test_subtract 0x1d)
add_test(NAME test_DCR_H COMMAND test_subtract 0x25)
add_test(NAME test_DCR_L COMMAND test_subtract 0x2d)
add_test(NAME test_DCR_M COMMAND test_subtract 0x35)
add_test(NAME test_DCX_B COMMAND test_subtract 0x0b)
add_test(NAME test_DCX_D COMMAND test_subtract 0x1b)
add_test(NAME test_DCX_H COMMAND test_subtract 0x2b)
add_test(NAME test_DCX_SP COMMAND test_subtract 0x3b)
add_test(NAME test_SUB_A COMMAND test_subtract 0x97)
add_test(NAME test_SUB_B COMMAND test_subtract 0x90)
add_test(NAME test_SUB_C COMMAND test_subtract 0x91)
add_test(NAME test_SUB_D COMMAND test_subtract 0x92)
add_test(NAME test_SUB_E COMMAND test_subtract 0x93)
add_test(NAME test_SUB_H COMMAND test_subtract 0x94)
add_test(NAME test_SUB_L COMMAND test_subtract 0x95)
add_test(NAME test_SUB_M COMMAND test_subtract 0x96)
add_test(NAME test_SBB_A COMMAND test_subtract 0x9f)
add_test(NAME test_SBB_B COMMAND test_subtract 0x98)
add_test(NAME test_SBB_C COMMAND test_subtract 0x99)
add_test(NAME test_SBB_D COMMAND test_subtract 0x9a)
add_test(NAME test_SBB_E COMMAND test_subtract 0x9b)
add_test(NAME test_SBB_H COMMAND test_subtract 0x9c)
add_test(NAME test_SBB_L COMMAND test_subtract 0x9d)
add_test(NAME test_SBB_M COMMAND test_subtract 0x9e)
add_test(NAME test_SBI COMMAND test_subtract 0xde)
add_test(NAME test_SUI COMMAND test_subtract 0xd6)
add_test(NAME test_subtract_helper COMMAND test_subtract 0xFFFF)

# Test Move Immediate Instructions
add_executable(test_move_immediate test_move_immediate.c)
add_test(NAME test_MVI_B COMMAND test_move_immediate 0x06)
add_test(NAME test_MVI_C COMMAND test_move_immediate 0x0e)
add_test(NAME test_MVI_D COMMAND test_move_immediate 0x16)
add_test(NAME test_MVI_E COMMAND test_move_immediate 0x1e)
add_test(NAME test_MVI_H COMMAND test_move_immediate 0x26)
add_test(NAME test_MVI_L COMMAND test_move_immediate 0x2e)
add_test(NAME test_MVI_M COMMAND test_move_immediate 0x36)
add_test(NAME test_MVI_A COMMAND test_move_immediate 0x3e)

# Test Rotate Instructions
add_executable(test_rotate test_rotate.c)
add_test(NAME test_RAL COMMAND test_rotate 0x17)
add_test(NAME test_RAR COMMAND test_rotate 0x1f)
add_test(NAME test_RLC COMMAND test_rotate 0x07)
add_test(NAME test_RRC COMMAND test_rotate 0x0f)


# Test Push/Pop Instructions
add_executable(test_push_pop test_push_pop.c)
add_test(NAME pop_b COMMAND test_push_pop 0xc1)
add_test(NAME push_b COMMAND test_push_pop 0xc5)
add_test(NAME test_POP_D, COMMAND test_push_pop 0xd1)
add_test(NAME test_PUSH_D, COMMAND test_push_pop 0xd5)
add_test(NAME test_POP_H, COMMAND test_push_pop 0xe1)
add_test(NAME test_PUSH_H, COMMAND test_push_pop 0xe5)
add_test(NAME test_POP_PSW, COMMAND test_push_pop 0xf1)
add_test(NAME test_PUSH_PSW, COMMAND test_push_pop 0xf5)

# Test Call Instructions
add_executable(test_call test_call.c)
add_test(NAME test_CALL, COMMAND test_call 0xcd)
add_test(NAME test_CNZ, COMMAND test_call 0xc4)
add_test(NAME test_CZ, COMMAND test_call 0xcc)
add_test(NAME test_CNC, COMMAND test_call 0xd4)
add_test(NAME test_CC, COMMAND test_call 0xdc)
add_test(NAME test_CPO, COMMAND test_call 0xe4)
add_test(NAME test_CPE COMMAND test_call 0xec)
add_test(NAME test_CP, COMMAND test_call 0xf4)
add_test(NAME test_CM, COMMAND test_call 0xfc)

add_executable(test_immediates test_immediates.c)
add_test(NAME test_ANI_D8, COMMAND test_immediates 0xe6)

add_executable(test_exchange test_exchange.c)
add_test(NAME test_XCHG, COMMAND test_exchange 0xeb)
add_test(NAME test_XTHL, COMMAND test_exchange 0xe3)

add_executable(test_compare test_compare.c)
add_test(NAME test_CPI_D8, COMMAND test_compare 0xfe)
add_test(NAME test_CMP_B, COMMAND test_compare 0xb8)
add_test(NAME test_CMP_C, COMMAND test_compare 0xb9)
add_test(NAME test_CMP_D, COMMAND test_compare 0xba)
add_test(NAME test_CMP_E, COMMAND test_compare 0xbb)
add_test(NAME test_CMP_H, COMMAND test_compare 0xbc)
add_test(NAME test_CMP_L, COMMAND test_compare 0xbd)
add_test(NAME test_CMP_M, COMMAND test_compare 0xbe)
add_test(NAME test_CMP_A, COMMAND test_compare 0xbf)

add_executable(test_complement test_complement.c)
add_test(NAME test_CMC, COMMAND test_complement 0x3f)
add_test(NAME test_CMA, COMMAND test_complement 0x2f)

add_executable(test_decimal_adjust test_decimal_adjust.c)
add_test(NAME test_DAA, COMMAND test_decimal_adjust 0x27)

# Test NOP
add_executable(test_nop test_nop.c)
add_test(NAME test_NOP, COMMAND test_nop 0x00)
add_test(NAME test_RIM, COMMAND test_nop 0x20)
add_test(NAME test_SIM, COMMAND test_nop 0x30)

add_executable(test_stc test_stc.c)
add_test(NAME test_STC, COMMAND test_stc 0x37)

add_executable(test_io_interrupts test_io_interrupts.c)
add_test(NAME test_EI, COMMAND test_io_interrupts 0xfb)
add_test(NAME test_DI, COMMAND test_io_interrupts 0xf3)
add_test(NAME test_HLT, COMMAND test_io_interrupts 0x76)
add_test(NAME test_RST_0, COMMAND test_io_interrupts 0xc7)
add_test(NAME test_RST_1, COMMAND test_io_interrupts 0xcf)
add_test(NAME test_RST_2, COMMAND test_io_interrupts 0xd7)
add_test(NAME test_RST_3, COMMAND test_io_interrupts 0xdf)
add_test(NAME test_RST_4, COMMAND test_io_interrupts 0xe7)
add_test(NAME test_RST_5, COMMAND test_io_interrupts 0xef)
add_test(NAME test_RST_6, COMMAND test_io_interrupts 0xf7)
add_test(NAME test_RST_7, COMMAND test_io_interrupts 0xff)
add_test(NAME test_IN, COMMAND test_io_interrupts 0xdb)
add_test(NAME test_OUT, COMMAND test_io_interrupts 0xd3)

add_executable(test_diagnostics_asm test_diagnostics_asm.c)
add_test(NAME diagnostic_asm, COMMAND test_diagnostics_asm)

if (EXISTS "${PROJECT_SOURCE_DIR}/include/invaders_combined")
    add_executable(test_state test_states.c)
    add_test(NAME test_state_at_10, COMMAND test_state 10)
    add_test(NAME test_state_at_15, COMMAND test_state 15)
    add_test(NAME test_state_at_25, COMMAND test_state 25)
    add_test(NAME test_state_at_100, COMMAND test_state 100)
    add_test(NAME test_state_at_1k, COMMAND test_state 1000)
    add_test(NAME test_state_at_10k, COMMAND test_state 10000)
    add_test(NAME test_state_at_25k, COMMAND test_state 25000)
    add_test(NAME test_state_at_37_5k, COMMAND test_state 37500)
    #add_test(NAME test_state_at_50k, COMMAND test_state 50000)
    #add_test(NAME test_state_at_100k, COMMAND test_state 100000)

    add_executable(test_sound test_sound.c)
    add_test(NAME test_sound1, COMMAND test_sound)
endif ()
