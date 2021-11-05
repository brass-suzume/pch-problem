project( Lib )

add_library( ${PROJECT_NAME} )

target_sources( ${PROJECT_NAME}
					PRIVATE
						LibFile.cpp

					PUBLIC
						LibFile.h )

target_precompile_headers( ${PROJECT_NAME} 
								PUBLIC
									LibFile.h )