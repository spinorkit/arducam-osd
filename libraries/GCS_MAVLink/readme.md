Current headers were generated for Pixhawk. "generates.sh" was not used.

mavlink_conversions.h had to be modified because of unavailable math functions:
(TODO: fix this properly)

    // added for compilation for Arduino
    #ifndef atanf
        #define atanf atan
    #endif
    
    #ifndef atan2f
        #define atan2f atan2
    #endif
    
    #ifndef fabsf
        #define fabsf fabs
    #endif

