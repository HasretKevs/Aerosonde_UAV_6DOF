All of the equations and values used in the model are taken from the "Small Unmanned Aircraft Theory and Practice by Randal W. Beard, Timothy W. McLain


%%%%%%%%%%%%%%%%%%%%%%% Airframe Parameters %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

m=13.5; % mass(kg)

Ix=0.8244; % Inertia along x axis (kg*m^2) 

Iy=1.135; % Inertia along y axis (kg*m^2) 

Iz=1.759; % Inertia along z axis (kg*m^2) 

Ixy=0; % Inertia on xy plane (kg*m^2) 

Iyz=0; % Inertia on yz plane (kg*m^2) 

Ixz=0.1204; % Inertia on xz plane (kg*m^2) 

I=[Ix -Ixy -Ixz;-Ixy Iy -Iyz;-Ixz -Iyz Iz]; % Inertia Matrix

S=0.55; % Surface Area (m^2)

b=2.8956; % Wingspan (m)

c=0.18994; % Chord (m)

Sprop=0.2027; % Propeller Surface Area (m^2)

k_motor=80; % Motor Constant

kTp=0; % Experimental Constant 

k_omega=0; % Propeller Rotation Constant

rho_SL=1.225; % Sea Level air Density(kg/m^3)

TrimCondition(1)=-3.0373; % Elevator Trim At 100 m (degree) 

TrimCondition(2)=0; % Aileron Trim At 100 m (degree) 

TrimCondition(3)=0; % Rudder Trim At 100 m (degree) 

TrimCondition(4)=0.45225; % Throttle Trim At 100 m 



%%%%%%%%%%%%%%%%%%%%% Longitudinal Coefficients %%%%%%%%%%%%%%%%%%%%%%%%%%%

CL0=0.28;

CD0=0.03;

Cm0=-0.02338;

dCLdalpha=3.45;

dCDdalpha=0.3;

dCmdalpha=-0.38;

dCLdq=0;

dCDdq=0;

dCmdq=-3.6;

dCLdsigmaE=-0.36;

dCDdsigmaE=0;

dCmdsigmaE=-0.5;

Cprop=1;

M=50;

alpha_0=0.4712;

epsilon=0.1592;

dCDdp=0.0437;

dCndsigmaR=-0.032;


%%%%%%%%%%%%%%%%%%%%%%%% Lateral Coefficients %%%%%%%%%%%%%%%%%%%%%%%%%%%%%

Cy0=0;

Cl0=0;

Cn0=0;

dCydbeta=-0.98;

dCldbeta=-0.12;

dCndbeta=0.25;

dCydp=0;

dCldp=-0.26;

dCndp=0.022

dCydr=0;

dCldr=0.14;

dCndr=-0.35;

dCydsigmaA=0;

dCldsigmaA=0.08;

dCndsigmaA=0.06;

dCydsigmaR=-0.17;

dCldsigmaR=-0.105;
