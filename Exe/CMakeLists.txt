project( Executable )

add_executable( ${PROJECT_NAME} )

target_sources( ${PROJECT_NAME}
					PRIVATE
						ExeFile.cpp

					PUBLIC
						ExeFile.h )
						
target_link_libraries( ${PROJECT_NAME} 
							PRIVATE
								Lib )

target_precompile_headers( ${PROJECT_NAME} 
								PUBLIC
									ExeFile.h )