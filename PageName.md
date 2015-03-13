# Introduction #

todo : Address EOT detection

# Details #
> Note to Systems Programmers:
> > ansitape uses a boolean function  (eot)  to  determine
> > when  the  tape  drive has hit the end of file.  It is
> > called every time a block of data is  written  to  the
> > tape.   If  this function ever returns TRUE (a defined
> > constant), an automatic  volume  switch  occurs.   The
> > pertinent  device registers are obtained by a MTIOCGET
> > ioctl system call.  The  registers  are  described  in
> > /sys/sundev/tmreg.h  (Sun  system with TapeMaster con-
> > troller).  If you have a VAX,  the  filename  will  be
> > slightly  different.   Sun  Microsystems supplies this
> > file even with binary-only distributions.