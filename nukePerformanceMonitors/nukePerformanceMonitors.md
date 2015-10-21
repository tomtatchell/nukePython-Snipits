#Nuke performance monitors
ptimeMenu = nuke.menu("Nodes").addMenu("Performance Timers", icon= "performanceTimer.png")
ptimeMenu.addCommand("Performance On", 'nuke.startPerformanceTimers()')
ptimeMenu.addCommand("Performance Off", 'nuke.stopPerformanceTimers()')
ptimeMenu.addCommand("Performance reset", 'nuke.resetPerformanceTimers()')
ptimeMenu.addCommand("Performance Status", 'nuke.message(str(nuke.usingPerformanceTimers()))')